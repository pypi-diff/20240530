# Comparing `tmp/pulumiverse_pulumi_dynatrace-0.3.0.tar.gz` & `tmp/pulumiverse_pulumi_dynatrace-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_pulumi_dynatrace-0.3.0.tar", last modified: Thu May 30 10:16:20 2024, max compression
+gzip compressed data, was "pulumiverse_pulumi_dynatrace-0.5.0.tar", last modified: Thu May 30 11:25:58 2024, max compression
```

## Comparing `pulumiverse_pulumi_dynatrace-0.3.0.tar` & `pulumiverse_pulumi_dynatrace-0.5.0.tar`

### file list

```diff
@@ -1,619 +1,619 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:19.946690 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/
--rw-r--r--   0 runner    (1001) docker     (127)    52793 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2882812 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/activegate_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/activegate_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aix_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/alerting_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31058 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ansible_tower_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/api_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25395 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/api_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_data_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_detection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_detection_rule_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_error_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/autotag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/autotag_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aws_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/azure_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    25339 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor_outage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_oneagent.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    39176 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/calculated_service_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloud_foundry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudapp_workloaddetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudfoundary_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudfoundry_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:19.950690 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/connectivity_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_builtin_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    21297 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    31763 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    41281 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_crash_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboard_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_general.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/data_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/database_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/database_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ddu_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/declarative_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23978 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomaly_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    24062 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_specific_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/email_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/eula_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/extension_execution_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/extension_execution_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/failure_detection_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/failure_detection_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/frequent_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)    25363 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/generic_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/generic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/geolocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_alerting_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_alerting_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_aws_iam_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_calculated_service_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_iam_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_management_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_management_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_mobile_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_process_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_request_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_request_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_slo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_synthetic_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_synthetic_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    66552 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_process_group_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_outage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20555 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_policy_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ibm_mq_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ims_bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/issue_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/jira_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/json_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_cluster_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    49873 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_namespace_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_node_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_pvc_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_workload_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/key_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    52067 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_custom_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_grail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    47869 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_oneagent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_sensitive_data_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mainframe_transaction_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22613 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    20005 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/management_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/management_zone_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mgmz_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_crash_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37224 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_apache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_dotnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_iis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_java.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_opentracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_php.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_varnish.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_wsmb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/muted_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/nettracer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_default_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/opentelemetry_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ops_genie_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39671 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/os_services.py
--rw-r--r--   0 runner    (1001) docker     (127)  2437368 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ownership_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28383 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ownership_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pager_duty_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pg_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pg_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/policy_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    66605 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_detection_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_rum.py
--rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_simple_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_monitoring_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    66840 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/processgroup_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/queue_sharing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/remote_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    23792 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_namings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/resource_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_advanced_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_host_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_ip_determination.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_ip_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_overload_prevention.py
--rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_provider_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    15739 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_external_web_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_external_web_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)    18502 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_full_web_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18502 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_full_web_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_http_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)    66660 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    34033 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_now_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/session_replay_resource_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/session_replay_web_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slack_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    28582 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    32107 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_attributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_capture_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/synthetic_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)    38391 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/synthetic_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/token_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/transaction_start_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    33857 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/trello_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    33879 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/trrello_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/update_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/usability_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_action_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_experience_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    19420 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_session_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/victor_ops_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/vmware_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_beacon_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)    11830 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_javascript_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_javascript_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_resource_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_resource_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    60440 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_application.py
--rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/webhook_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/xmatters_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/
--rw-r--r--   0 runner    (1001) docker     (127)    73598 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  4567024 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/activegate_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/activegate_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    20099 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ag_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aix_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    34956 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/alerting_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31058 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ansible_tower_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/api_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25395 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/api_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/app_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_data_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_detection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_detection_rule_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_error_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    54590 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/appsec_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_block_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attributes_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    77223 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_business_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)   253164 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_scheduling_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    30591 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow_jira.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    32882 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    47820 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/azure_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/azure_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25392 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor_outage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)   161693 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/builtin_process_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_oneagent.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_security_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    22551 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_mobile_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    41600 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_service_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    24893 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_synthetic_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    22222 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_web_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloud_foundry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloudapp_workloaddetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloudfoundry_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/connectivity_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_builtin_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17957 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/crashdump_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    37087 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    42472 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_crash_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboard_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_general.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    18230 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/data_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/database_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/database_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/davis_anomaly_detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/db_app_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ddu_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/declarative_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/direct_shares.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23978 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomaly_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    24062 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_specific_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ebpf_service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/email_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/eula_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/extension_execution_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/extension_execution_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/failure_detection_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/failure_detection_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/frequent_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)    25363 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/geolocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_alerting_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_alerting_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_attack_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_iam_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_supported_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_azure_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_azure_supported_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_calculated_service_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_failure_detection_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_hub_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_lambda_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zone_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_mobile_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_process_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_remote_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_request_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_request_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_slo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_update_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_vulnerability_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_security_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16906 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    66552 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_process_group_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    24572 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_outage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_extension_active_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_extension_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    22019 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17930 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ibm_mq_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ims_bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/infraops_app_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ip_address_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    28446 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/issue_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/jira_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/json_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/json_dashboard_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_cluster_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    49873 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    29566 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_namespace_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_node_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_pvc_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    45135 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_workload_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/key_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/key_user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    65252 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/kubernetes_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/limit_outbound_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_custom_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_debug_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_grail.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    47560 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_oneagent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_security_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_sensitive_data_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    17664 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    22146 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mainframe_transaction_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    29435 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_internet_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    25371 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_network_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    41603 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_public_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_remote_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_smtp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20005 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/management_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/management_zone_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19274 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mgmz_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_crash_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_key_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    36972 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_apache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_dotnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_iis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_java.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nginx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_opentracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_php.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_varnish.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_wsmb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/muted_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/nettracer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_default_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_side_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/opentelemetry_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ops_genie_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    43259 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/os_services.py
--rw-r--r--   0 runner    (1001) docker     (127)  4061938 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ownership_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28173 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ownership_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pager_duty_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pg_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pg_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/platform_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/policy_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)    19107 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    66605 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_detection_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_rum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_simple_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_monitoring_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    66840 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/processgroup_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/queue_sharing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/remote_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    23792 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_namings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/resource_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_advanced_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_host_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_ip_determination.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_ip_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_overload_prevention.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_provider_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    15739 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_anomalies_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_external_web_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_external_web_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_full_web_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_full_web_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_http_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)    66660 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    36715 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_now_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/session_replay_resource_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/session_replay_web_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/site_reliability_guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slack_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    34400 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    32056 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_attributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_capture_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/synthetic_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)    46414 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/synthetic_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/token_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/transaction_start_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    34078 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/trello_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/unified_services_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/unified_services_opentel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/update_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)    31778 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/url_based_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/usability_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_action_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_experience_score.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_session_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19793 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/victor_ops_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vmware.py
--rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vmware_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    21583 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_third_party.py
--rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_beacon_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_beacon_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_custom_config_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    11830 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)    18452 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_injection_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_javascript_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_javascript_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_xhr.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_resource_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14606 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_resource_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    62301 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_application.py
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/webhook_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/xmatters_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:16:20.010690 pulumiverse_pulumi_dynatrace-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 10:16:19.000000 pulumiverse_pulumi_dynatrace-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.770448 pulumiverse_pulumi_dynatrace-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 11:25:58.770448 pulumiverse_pulumi_dynatrace-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.702448 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/
+-rw-r--r--   0 runner    (1001) docker     (127)    52793 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2882812 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/activegate_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/activegate_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aix_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/alerting_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31058 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ansible_tower_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/api_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25395 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/api_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_data_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_detection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_detection_rule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_error_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/autotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/autotag_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aws_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/azure_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25339 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor_outage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_oneagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39176 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/calculated_service_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloud_foundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudapp_workloaddetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21460 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudfoundary_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudfoundry_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.702448 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/connectivity_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_builtin_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14292 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21297 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31763 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41281 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_crash_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboard_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/data_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/database_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/database_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16685 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ddu_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/declarative_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23978 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomaly_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24062 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_specific_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/email_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/eula_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/extension_execution_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/extension_execution_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/failure_detection_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/failure_detection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/frequent_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25363 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/generic_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/generic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/geolocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_alerting_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_alerting_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_aws_iam_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_calculated_service_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_management_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_management_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_mobile_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_process_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_request_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_request_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_synthetic_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_synthetic_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66552 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_process_group_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_outage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20555 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_policy_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19433 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ibm_mq_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ims_bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24781 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/issue_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/jira_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/json_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_cluster_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49873 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_namespace_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_node_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_pvc_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_workload_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/key_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52067 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_custom_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_grail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14468 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47869 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_oneagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_sensitive_data_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mainframe_transaction_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22613 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20005 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/management_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/management_zone_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mgmz_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_crash_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37224 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_apache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_opentracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_varnish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_wsmb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/muted_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/nettracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_default_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30612 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/opentelemetry_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ops_genie_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39671 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/os_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2437368 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ownership_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28383 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ownership_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pager_duty_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pg_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pg_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/policy_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66605 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_detection_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_rum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_simple_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_monitoring_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66840 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/processgroup_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/queue_sharing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/remote_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23792 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_namings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/resource_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_advanced_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_host_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_ip_determination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_ip_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_overload_prevention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15708 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_provider_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15739 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_external_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_external_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18502 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_full_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18502 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_full_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_http_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66660 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34033 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_now_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/session_replay_resource_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/session_replay_web_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slack_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28582 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32107 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_attributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_capture_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/synthetic_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38391 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/synthetic_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/token_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/transaction_start_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33857 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/trello_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33879 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/trrello_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/update_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/usability_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_action_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_experience_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19420 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_session_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/victor_ops_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/vmware_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_beacon_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11830 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_javascript_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_javascript_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_resource_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_resource_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60440 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34678 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/webhook_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/xmatters_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.766448 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/
+-rw-r--r--   0 runner    (1001) docker     (127)    73598 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4567024 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/activegate_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/activegate_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20099 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ag_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aix_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34956 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/alerting_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31058 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ansible_tower_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17784 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/api_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25395 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/api_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/app_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18817 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_data_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_detection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16157 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_detection_rule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_error_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54590 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/appsec_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_block_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attributes_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77223 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_business_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253164 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_scheduling_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30591 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow_jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29598 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32882 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47820 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/azure_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/azure_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25392 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor_outage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161693 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/builtin_process_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19266 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_oneagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_security_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22551 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_mobile_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41600 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_service_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24893 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_synthetic_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22222 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_web_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloud_foundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloudapp_workloaddetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloudfoundry_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.770448 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/connectivity_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_builtin_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17957 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/crashdump_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37087 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42472 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_crash_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9821 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboard_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18230 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/data_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/database_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20051 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/database_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/davis_anomaly_detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/db_app_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ddu_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/declarative_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/direct_shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23978 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomaly_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24062 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_specific_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ebpf_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33590 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/email_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/eula_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/extension_execution_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/extension_execution_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/failure_detection_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/failure_detection_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/frequent_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25363 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/geolocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_alerting_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_alerting_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_attack_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_iam_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_supported_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_azure_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_azure_supported_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_calculated_service_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_failure_detection_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_hub_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_lambda_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zone_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_mobile_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_process_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_remote_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_request_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_request_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_update_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_vulnerability_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_security_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16906 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66552 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_process_group_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24572 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_outage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_extension_active_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_extension_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22019 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17930 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ibm_mq_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ims_bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/infraops_app_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ip_address_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28446 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/issue_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34133 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/jira_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/json_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/json_dashboard_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_cluster_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49873 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29566 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_namespace_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20781 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_node_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_pvc_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45135 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_workload_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/key_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/key_user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65252 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/kubernetes_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/limit_outbound_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14382 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_custom_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_debug_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_grail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47560 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_oneagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_security_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17904 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_sensitive_data_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17664 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22146 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mainframe_transaction_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29435 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_internet_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25371 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_network_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41603 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_public_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_smtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20005 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/management_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/management_zone_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19274 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mgmz_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17270 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_crash_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_key_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36972 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_apache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_iis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_opentracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_php.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_varnish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_wsmb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/muted_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/nettracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30487 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_default_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_side_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/opentelemetry_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ops_genie_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43259 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/os_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4061938 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ownership_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28173 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ownership_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pager_duty_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pg_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pg_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/platform_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/policy_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19107 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66605 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_detection_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_rum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18898 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_simple_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16084 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_monitoring_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66840 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/processgroup_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/queue_sharing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/remote_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23792 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_namings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/resource_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_advanced_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_host_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_ip_determination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_ip_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_overload_prevention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_provider_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15739 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_anomalies_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_external_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_external_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_full_web_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_full_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_http_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66660 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36715 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_now_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/session_replay_resource_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/session_replay_web_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/site_reliability_guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25493 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slack_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34400 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32056 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_attributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_capture_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/synthetic_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46414 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/synthetic_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/token_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/transaction_start_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34078 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/trello_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/unified_services_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/unified_services_opentel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/update_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31778 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/url_based_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/usability_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_action_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_experience_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_session_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19793 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/victor_ops_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vmware_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21583 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16763 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_beacon_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_beacon_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_custom_config_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11830 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18452 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_injection_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9133 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_javascript_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_javascript_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_xhr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_resource_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14606 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_resource_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62301 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/webhook_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/xmatters_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:25:58.770448 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30148 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:25:58.770448 pulumiverse_pulumi_dynatrace-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-30 11:25:58.000000 pulumiverse_pulumi_dynatrace-0.5.0/setup.py
```

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/PKG-INFO` & `pulumiverse_pulumi_dynatrace-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_pulumi_dynatrace
-Version: 0.3.0
+Version: 0.5.0
 Summary: A Pulumi package for creating and managing Dynatrace cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-dynatrace
 Keywords: pulumi dynatrace category/infrastructure pulumiverse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/README.md` & `pulumiverse_pulumi_dynatrace-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/__init__.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/_inputs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/_utilities.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/activegate_token.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/activegate_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/activegate_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/activegate_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aix_extension.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aix_extension.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/alerting_profile.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/alerting_profile.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ansible_tower_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ansible_tower_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/api_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/api_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/api_token.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/api_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_data_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_data_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_detection_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_detection_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_detection_rule_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_detection_rule_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/application_error_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/application_error_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/audit_log.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/audit_log.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/autotag.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/autotag.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/autotag_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/autotag_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aws_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aws_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/aws_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/azure_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/azure_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor_outage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor_outage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/browser_monitor_performance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/browser_monitor_performance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_buckets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_buckets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_oneagent.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_oneagent.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/business_events_processing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/business_events_processing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/calculated_service_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/calculated_service_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloud_foundry.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloud_foundry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudapp_workloaddetection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudapp_workloaddetection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudfoundary_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudfoundary_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/cloudfoundry_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/cloudfoundry_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/config/vars.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/connectivity_alerts.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/connectivity_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_builtin_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_builtin_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/container_technology.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/container_technology.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_crash_rate.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_crash_rate.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_tags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_tags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/custom_units.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/custom_units.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboard_sharing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboard_sharing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_allowlist.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_general.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_general.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/dashboards_presets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/dashboards_presets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/data_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/data_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/database_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/database_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/database_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/database_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ddu_pool.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ddu_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/declarative_grouping.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/declarative_grouping.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_analytics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_anomaly_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_anomaly_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_options.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_options.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/disk_specific_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/disk_specific_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/email_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/email_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/environment.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/eula_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/eula_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/extension_execution_controller.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/extension_execution_controller.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/extension_execution_remote.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/extension_execution_remote.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/failure_detection_parameters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/failure_detection_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/failure_detection_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/failure_detection_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/frequent_issues.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/frequent_issues.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/generic_relationships.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/generic_relationships.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/generic_types.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/generic_types.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/geolocation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/geolocation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_alerting_profile.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_alerting_profile.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_alerting_profiles.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_alerting_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_aws_iam_external.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_aws_iam_external.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_calculated_service_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_calculated_service_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_entities.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_entities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_entity.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_host.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_iam_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_iam_user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_management_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_management_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_management_zones.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_management_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_mobile_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_mobile_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_process.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_process.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_process_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_process_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_request_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_request_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_request_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_request_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_slo.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_slo.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_synthetic_location.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_synthetic_location.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/get_synthetic_locations.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/get_synthetic_locations.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/host_process_group_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/host_process_group_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_cookies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_cookies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_outage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_outage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/http_monitor_performance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/http_monitor_performance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_permission.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_policy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_policy_bindings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_policy_bindings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/iam_user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ibm_mq_filters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ibm_mq_filters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ims_bridges.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ims_bridges.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/issue_tracking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/issue_tracking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/jira_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/jira_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/json_dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/json_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_cluster_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_cluster_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_namespace_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_namespace_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_node_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_node_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_pvc_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_pvc_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/k8s_workload_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/k8s_workload_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/key_requests.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/key_requests.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/kubernetes.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_buckets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_buckets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_custom_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_custom_source.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_custom_source.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_events.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_events.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_grail.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_grail.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_oneagent.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_oneagent.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_processing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_processing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_sensitive_data_masking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_sensitive_data_masking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_storage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_storage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/log_timestamp.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/log_timestamp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mainframe_transaction_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mainframe_transaction_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/maintenance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/maintenance_window.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/management_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/management_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/management_zone_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/management_zone_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_events.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_events.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_metadata.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/metric_query.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/metric_query.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mgmz_permission.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mgmz_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_crash_rate.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_crash_rate.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_app_request_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_app_request_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/mobile_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/mobile_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_apache.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_apache.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_dotnet.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_dotnet.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_go.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_go.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_iis.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_iis.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_java.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_java.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nginx.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nginx.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nodejs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_nodejs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_opentracing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_opentracing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_php.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_php.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_varnish.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_varnish.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/monitored_technologies_wsmb.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/monitored_technologies_wsmb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/muted_requests.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/muted_requests.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/nettracer.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/nettracer.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_traffic.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_traffic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/network_zones.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/network_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_default_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_default_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_features.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_features.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/oneagent_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/oneagent_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/opentelemetry_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/opentelemetry_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ops_genie_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ops_genie_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/os_services.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/os_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/outputs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ownership_config.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ownership_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/ownership_teams.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/ownership_teams.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pager_duty_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pager_duty_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pg_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pg_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/pg_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/pg_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/policy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/policy_bindings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/policy_bindings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_availability.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_availability.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_detection_flags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_detection_flags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_rum.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_rum.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_group_simple_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_group_simple_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_monitoring_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_monitoring_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/process_visibility.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/process_visibility.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/processgroup_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/processgroup_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/provider.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/queue_manager.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/queue_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/queue_sharing_groups.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/queue_sharing_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/remote_environments.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/remote_environments.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/request_namings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/request_namings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/resource_attributes.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_advanced_correlation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_advanced_correlation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_host_headers.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_host_headers.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_ip_determination.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_ip_determination.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_ip_locations.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_ip_locations.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_overload_prevention.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_overload_prevention.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/rum_provider_breakdown.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/rum_provider_breakdown.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_external_web_request.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_external_web_request.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_external_web_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_external_web_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_failure.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_failure.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_full_web_request.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_full_web_request.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_full_web_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_full_web_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_http_failure.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_http_failure.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/service_now_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/service_now_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/session_replay_resource_capture.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/session_replay_resource_capture.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/session_replay_web_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/session_replay_web_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slack_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slack_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo_normalization.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo_normalization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/slo_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/slo_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_attributed.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_attributed.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_capture_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_capture_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_context_propagation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_context_propagation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/span_entry_point.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/span_entry_point.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/synthetic_availability.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/synthetic_availability.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/synthetic_location.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/synthetic_location.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/token_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/token_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/transaction_start_filters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/transaction_start_filters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/trello_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/trello_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/trrello_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/trrello_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/update_windows.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/update_windows.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/usability_analytics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/usability_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_action_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_action_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_experience_score.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_experience_score.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_session_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_session_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/user_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/user_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/victor_ops_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/victor_ops_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/vmware_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/vmware_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_beacon_origins.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_beacon_origins.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_custom_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_custom_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_javascript_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_javascript_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_javascript_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_javascript_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_request_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_request_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_resource_cleanup.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_resource_cleanup.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_app_resource_types.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_app_resource_types.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/web_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/web_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/webhook_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/lbrlabs_pulumi_dynatrace/xmatters_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/lbrlabs_pulumi_dynatrace/xmatters_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/__init__.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/_inputs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/_utilities.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/activegate_token.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/activegate_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/activegate_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/activegate_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ag_token.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ag_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aix_extension.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aix_extension.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/alerting_profile.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/alerting_profile.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ansible_tower_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ansible_tower_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/api_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/api_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/api_token.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/api_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/app_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/app_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_data_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_data_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_detection_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_detection_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_detection_rule_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_detection_rule_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/application_error_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/application_error_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/appsec_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/appsec_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_allowlist.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attack_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attack_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_allow_list.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_block_list.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_block_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attribute_masking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attribute_masking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/attributes_preferences.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/attributes_preferences.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/audit_log.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/audit_log.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_business_calendar.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_business_calendar.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_scheduling_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_scheduling_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow_jira.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow_jira.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/automation_workflow_slack.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/automation_workflow_slack.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/autotag_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/autotag_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/aws_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/aws_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/azure_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/azure_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/azure_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/azure_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor_outage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor_outage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/browser_monitor_performance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/browser_monitor_performance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/builtin_process_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/builtin_process_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_buckets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_buckets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_oneagent.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_oneagent.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_processing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_processing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/business_events_security_context.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/business_events_security_context.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_mobile_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_mobile_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_service_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_service_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_synthetic_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_synthetic_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/calculated_web_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/calculated_web_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloud_foundry.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloud_foundry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloudapp_workloaddetection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloudapp_workloaddetection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/cloudfoundry_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/cloudfoundry_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/config/vars.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/connectivity_alerts.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/connectivity_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_builtin_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_builtin_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_registry.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/container_technology.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/container_technology.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/crashdump_analytics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/crashdump_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_crash_rate.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_crash_rate.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_device.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_device.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_tags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_tags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/custom_units.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/custom_units.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboard_sharing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboard_sharing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_allowlist.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_general.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_general.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/dashboards_presets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/dashboards_presets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/data_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/data_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/database_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/database_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/database_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/database_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/davis_anomaly_detectors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/davis_anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/db_app_feature_flags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/db_app_feature_flags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ddu_pool.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ddu_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/declarative_grouping.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/declarative_grouping.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/direct_shares.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/direct_shares.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_analytics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_anomaly_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_anomaly_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_options.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_options.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/disk_specific_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/disk_specific_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/document.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/document.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ebpf_service_discovery.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ebpf_service_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/email_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/email_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/environment.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/eula_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/eula_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/extension_execution_controller.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/extension_execution_controller.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/extension_execution_remote.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/extension_execution_remote.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/failure_detection_parameters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/failure_detection_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/failure_detection_rules.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/failure_detection_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/frequent_issues.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/frequent_issues.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_relationships.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_relationships.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_setting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_setting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/generic_types.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/generic_types.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/geolocation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/geolocation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_alerting_profile.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_alerting_profile.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_alerting_profiles.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_alerting_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_attack_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_attack_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_iam_external.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_iam_external.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_aws_supported_services.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_aws_supported_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_azure_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_azure_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_azure_supported_services.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_azure_supported_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_calculated_service_metric.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_calculated_service_metric.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_documents.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_documents.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_entities.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_entities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_entity.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_failure_detection_parameters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_failure_detection_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_host.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_hub_items.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_hub_items.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_groups.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_policies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_policies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_policy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_iam_user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_lambda_agent_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_lambda_agent_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zone_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zone_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_management_zones.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_management_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_mobile_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_mobile_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_process.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_process.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_process_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_process_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_remote_environments.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_remote_environments.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_request_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_request_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_request_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_request_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_slo.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_slo.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_location.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_location.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_locations.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_locations.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_synthetic_nodes.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_synthetic_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_tenant.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_update_windows.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_update_windows.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/get_vulnerability_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/get_vulnerability_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowall.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowall.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowlist.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_metrics_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/grail_security_context.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/grail_security_context.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring_advanced.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring_advanced.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_monitoring_mode.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_monitoring_mode.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/host_process_group_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/host_process_group_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_cookies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_cookies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_outage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_outage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_performance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_performance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/http_monitor_script.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/http_monitor_script.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_extension_active_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_extension_active_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_extension_config.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_extension_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/hub_subscriptions.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/hub_subscriptions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_permission.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_policy_bindings_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/iam_user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/iam_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ibm_mq_filters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ibm_mq_filters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ims_bridges.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ims_bridges.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/infraops_app_feature_flags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/infraops_app_feature_flags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ip_address_masking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ip_address_masking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/issue_tracking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/issue_tracking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/jira_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/jira_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/json_dashboard.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/json_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/json_dashboard_base.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/json_dashboard_base.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_cluster_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_cluster_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_credentials.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_namespace_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_namespace_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_node_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_node_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_pvc_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_pvc_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/k8s_workload_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/k8s_workload_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/key_requests.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/key_requests.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/key_user_action.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/key_user_action.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/kubernetes.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/kubernetes_app.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/limit_outbound_connections.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/limit_outbound_connections.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_buckets.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_buckets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_custom_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_custom_source.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_custom_source.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_debug_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_debug_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_events.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_events.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_grail.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_grail.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_oneagent.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_oneagent.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_processing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_processing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_security_context.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_security_context.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_sensitive_data_masking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_sensitive_data_masking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_storage.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_storage.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/log_timestamp.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/log_timestamp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mainframe_transaction_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mainframe_transaction_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/maintenance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/maintenance_window.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_backup.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_backup.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_internet_proxy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_internet_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_network_zones.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_network_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_preferences.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_preferences.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_public_endpoints.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_public_endpoints.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_remote_access.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_remote_access.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/managed_smtp.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/managed_smtp.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/management_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/management_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/management_zone_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/management_zone_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_events.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_events.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_metadata.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/metric_query.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/metric_query.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mgmz_permission.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mgmz_permission.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_crash_rate.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_crash_rate.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_key_performance.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_key_performance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_app_request_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_app_request_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/mobile_notifications.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/mobile_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_apache.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_apache.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_dotnet.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_dotnet.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_go.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_go.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_iis.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_iis.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_java.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_java.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nginx.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nginx.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nodejs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_nodejs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_opentracing.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_opentracing.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_php.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_php.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_varnish.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_varnish.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/monitored_technologies_wsmb.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/monitored_technologies_wsmb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/muted_requests.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/muted_requests.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/nettracer.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/nettracer.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_traffic.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_traffic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_zone.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/network_zones.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/network_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_default_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_default_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_features.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_features.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_side_masking.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_side_masking.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/oneagent_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/oneagent_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/opentelemetry_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/opentelemetry_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ops_genie_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ops_genie_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/os_services.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/os_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/outputs.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ownership_config.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ownership_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/ownership_teams.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/ownership_teams.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pager_duty_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pager_duty_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pg_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pg_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/pg_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/pg_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/platform_bucket.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/platform_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/policy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/policy_bindings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/policy_bindings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_availability.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_availability.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_detection_flags.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_detection_flags.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_rum.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_rum.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_group_simple_detection.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_group_simple_detection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_monitoring.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_monitoring.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_monitoring_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_monitoring_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/process_visibility.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/process_visibility.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/processgroup_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/processgroup_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/provider.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/queue_manager.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/queue_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/queue_sharing_groups.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/queue_sharing_groups.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/remote_environments.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/remote_environments.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_attribute.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/request_namings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/request_namings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/resource_attributes.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_advanced_correlation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_advanced_correlation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_host_headers.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_host_headers.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_ip_determination.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_ip_determination.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_ip_locations.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_ip_locations.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_overload_prevention.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_overload_prevention.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/rum_provider_breakdown.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/rum_provider_breakdown.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_anomalies_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_anomalies_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_external_web_request.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_external_web_request.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_external_web_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_external_web_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_failure.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_failure.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_full_web_request.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_full_web_request.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_full_web_service.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_full_web_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_http_failure.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_http_failure.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_naming.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_naming.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/service_now_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/service_now_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/session_replay_resource_capture.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/session_replay_resource_capture.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/session_replay_web_privacy.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/session_replay_web_privacy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/site_reliability_guardian.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/site_reliability_guardian.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slack_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slack_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo_normalization.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo_normalization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/slo_v2.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/slo_v2.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_attributed.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_attributed.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_capture_rule.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_capture_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_context_propagation.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_context_propagation.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_entry_point.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_entry_point.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/span_events.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/span_events.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/synthetic_availability.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/synthetic_availability.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/synthetic_location.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/synthetic_location.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/token_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/token_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/transaction_start_filters.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/transaction_start_filters.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/trello_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/trello_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/unified_services_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/unified_services_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/unified_services_opentel.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/unified_services_opentel.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/update_windows.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/update_windows.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/url_based_sampling.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/url_based_sampling.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/usability_analytics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/usability_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_action_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_action_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_experience_score.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_experience_score.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_group.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_session_metrics.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_session_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/user_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/user_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/victor_ops_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/victor_ops_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vmware.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vmware.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vmware_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vmware_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_alerting.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_alerting.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_code.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_code.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_settings.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/vulnerability_third_party.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/vulnerability_third_party.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_anomalies.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_anomalies.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_beacon_endpoint.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_beacon_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_beacon_origins.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_beacon_origins.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_custom_config_properties.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_custom_config_properties.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_custom_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_custom_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_enablement.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_injection_cookie.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_injection_cookie.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_javascript_updates.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_javascript_updates.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_javascript_version.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_javascript_version.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_custom.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_custom.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_load.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_load.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_xhr.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_key_performance_xhr.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_request_errors.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_request_errors.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_resource_cleanup.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_resource_cleanup.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_app_resource_types.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_app_resource_types.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/web_application.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/web_application.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/webhook_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace/xmatters_notification.py` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace/xmatters_notification.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/PKG-INFO` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-pulumi-dynatrace
-Version: 0.3.0
+Version: 0.5.0
 Summary: A Pulumi package for creating and managing Dynatrace cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-dynatrace
 Keywords: pulumi dynatrace category/infrastructure pulumiverse
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/pulumiverse_pulumi_dynatrace.egg-info/SOURCES.txt` & `pulumiverse_pulumi_dynatrace-0.5.0/pulumiverse_pulumi_dynatrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_pulumi_dynatrace-0.3.0/setup.py` & `pulumiverse_pulumi_dynatrace-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.3.0"
+VERSION = "0.5.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "dynatrace Pulumi Package - Development Version"
```

