# Comparing `tmp/googleapis-common-protos-1.63.0.tar.gz` & `tmp/googleapis-common-protos-1.63.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapis-common-protos-1.63.0.tar", last modified: Mon Mar 11 12:33:12 2024, max compression
+gzip compressed data, was "googleapis-common-protos-1.63.1rc0.tar", last modified: Thu May 30 18:44:32 2024, max compression
```

## Comparing `googleapis-common-protos-1.63.0.tar` & `googleapis-common-protos-1.63.1rc0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.645857 googleapis-common-protos-1.63.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     1529 2024-03-11 12:33:12.645857 googleapis-common-protos-1.63.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003      362 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.605855 googleapis-common-protos-1.63.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.625856 googleapis-common-protos-1.63.0/google/api/
--rw-rw-r--   0 root         (0)     1003     1045 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/annotations.proto
--rw-rw-r--   0 root         (0)     1003     2133 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/annotations_pb2.py
--rw-rw-r--   0 root         (0)     1003     9257 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/auth.proto
--rw-rw-r--   0 root         (0)     1003     5613 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/auth_pb2.py
--rw-rw-r--   0 root         (0)     1003     7014 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/backend.proto
--rw-rw-r--   0 root         (0)     1003     4838 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/backend_pb2.py
--rw-rw-r--   0 root         (0)     1003     3062 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/billing.proto
--rw-rw-r--   0 root         (0)     1003     2933 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/billing_pb2.py
--rw-rw-r--   0 root         (0)     1003    14713 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/client.proto
--rw-rw-r--   0 root         (0)     1003    17267 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/client_pb2.py
--rw-rw-r--   0 root         (0)     1003     3166 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/config_change.proto
--rw-rw-r--   0 root         (0)     1003     3374 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/config_change_pb2.py
--rw-rw-r--   0 root         (0)     1003     2717 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/consumer.proto
--rw-rw-r--   0 root         (0)     1003     3138 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/consumer_pb2.py
--rw-rw-r--   0 root         (0)     1003     3067 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/context.proto
--rw-rw-r--   0 root         (0)     1003     2844 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/context_pb2.py
--rw-rw-r--   0 root         (0)     1003     1436 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/control.proto
--rw-rw-r--   0 root         (0)     1003     2300 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/control_pb2.py
--rw-rw-r--   0 root         (0)     1003     8660 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/distribution.proto
--rw-rw-r--   0 root         (0)     1003     7845 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/distribution_pb2.py
--rw-rw-r--   0 root         (0)     1003     6940 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/documentation.proto
--rw-rw-r--   0 root         (0)     1003     3698 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/documentation_pb2.py
--rw-rw-r--   0 root         (0)     1003     3028 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/endpoint.proto
--rw-rw-r--   0 root         (0)     1003     2380 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/endpoint_pb2.py
--rw-rw-r--   0 root         (0)     1003    22644 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/error_reason.proto
--rw-rw-r--   0 root         (0)     1003     4267 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/error_reason_pb2.py
--rw-rw-r--   0 root         (0)     1003     4306 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/field_behavior.proto
--rw-rw-r--   0 root         (0)     1003     2973 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/field_behavior_pb2.py
--rw-rw-r--   0 root         (0)     1003     3156 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/field_info.proto
--rw-rw-r--   0 root         (0)     1003     2920 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/field_info_pb2.py
--rw-rw-r--   0 root         (0)     1003    15159 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/http.proto
--rw-rw-r--   0 root         (0)     1003     3701 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/http_pb2.py
--rw-rw-r--   0 root         (0)     1003     2693 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/httpbody.proto
--rw-rw-r--   0 root         (0)     1003     2344 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/httpbody_pb2.py
--rw-rw-r--   0 root         (0)     1003     1389 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/label.proto
--rw-rw-r--   0 root         (0)     1003     2581 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/label_pb2.py
--rw-rw-r--   0 root         (0)     1003     3083 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/launch_stage.proto
--rw-rw-r--   0 root         (0)     1003     2277 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/launch_stage_pb2.py
--rw-rw-r--   0 root         (0)     1003     2043 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/log.proto
--rw-rw-r--   0 root         (0)     1003     2402 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/log_pb2.py
--rw-rw-r--   0 root         (0)     1003     3174 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/logging.proto
--rw-rw-r--   0 root         (0)     1003     3014 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/logging_pb2.py
--rw-rw-r--   0 root         (0)     1003    10605 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/metric.proto
--rw-rw-r--   0 root         (0)     1003     6432 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/metric_pb2.py
--rw-rw-r--   0 root         (0)     1003     5920 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/monitored_resource.proto
--rw-rw-r--   0 root         (0)     1003     6324 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/monitored_resource_pb2.py
--rw-rw-r--   0 root         (0)     1003     4457 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/monitoring.proto
--rw-rw-r--   0 root         (0)     1003     3129 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/monitoring_pb2.py
--rw-rw-r--   0 root         (0)     1003     3254 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/policy.proto
--rw-rw-r--   0 root         (0)     1003     3608 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/policy_pb2.py
--rw-rw-r--   0 root         (0)     1003     7138 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/quota.proto
--rw-rw-r--   0 root         (0)     1003     5303 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/quota_pb2.py
--rw-rw-r--   0 root         (0)     1003     8744 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/resource.proto
--rw-rw-r--   0 root         (0)     1003     4870 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/resource_pb2.py
--rw-rw-r--   0 root         (0)     1003    14929 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/routing.proto
--rw-rw-r--   0 root         (0)     1003     3189 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/routing_pb2.py
--rw-rw-r--   0 root         (0)     1003     6762 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/service.proto
--rw-rw-r--   0 root         (0)     1003     5979 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/service_pb2.py
--rw-rw-r--   0 root         (0)     1003     1091 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/source_info.proto
--rw-rw-r--   0 root         (0)     1003     2292 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/source_info_pb2.py
--rw-rw-r--   0 root         (0)     1003     3475 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/system_parameter.proto
--rw-rw-r--   0 root         (0)     1003     3583 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/system_parameter_pb2.py
--rw-rw-r--   0 root         (0)     1003     3787 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/usage.proto
--rw-rw-r--   0 root         (0)     1003     2791 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/usage_pb2.py
--rw-rw-r--   0 root         (0)     1003     3799 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/visibility.proto
--rw-rw-r--   0 root         (0)     1003     4956 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/api/visibility_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.625856 googleapis-common-protos-1.63.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003     6308 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/cloud/extended_operations.proto
--rw-rw-r--   0 root         (0)     1003     4032 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/cloud/extended_operations_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.625856 googleapis-common-protos-1.63.0/google/cloud/location/
--rw-rw-r--   0 root         (0)     1003     3604 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/cloud/location/locations.proto
--rw-rw-r--   0 root         (0)     1003     6899 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/cloud/location/locations_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.605855 googleapis-common-protos-1.63.0/google/gapic/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.629856 googleapis-common-protos-1.63.0/google/gapic/metadata/
--rw-rw-r--   0 root         (0)     1003     3393 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/gapic/metadata/gapic_metadata.proto
--rw-rw-r--   0 root         (0)     1003     8346 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/gapic/metadata/gapic_metadata_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.605855 googleapis-common-protos-1.63.0/google/logging/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.629856 googleapis-common-protos-1.63.0/google/logging/type/
--rw-rw-r--   0 root         (0)     1003     3601 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/logging/type/http_request.proto
--rw-rw-r--   0 root         (0)     1003     3176 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/logging/type/http_request_pb2.py
--rw-rw-r--   0 root         (0)     1003     2555 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/logging/type/log_severity.proto
--rw-rw-r--   0 root         (0)     1003     2622 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/logging/type/log_severity_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.629856 googleapis-common-protos-1.63.0/google/longrunning/
--rw-rw-r--   0 root         (0)     1003    10513 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations.proto
--rw-rw-r--   0 root         (0)     1003      797 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_grpc.py
--rw-rw-r--   0 root         (0)     1003      914 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_grpc_pb2.py
--rw-rw-r--   0 root         (0)     1003     2253 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_pb2.py
--rw-rw-r--   0 root         (0)     1003    14464 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0)     1003      222 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_proto.py
--rw-rw-r--   0 root         (0)     1003    10443 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/longrunning/operations_proto_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.633857 googleapis-common-protos-1.63.0/google/rpc/
--rw-rw-r--   0 root         (0)     1003     7138 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/code.proto
--rw-rw-r--   0 root         (0)     1003     2707 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/code_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.633857 googleapis-common-protos-1.63.0/google/rpc/context/
--rw-rw-r--   0 root         (0)     1003    14852 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/context/attribute_context.proto
--rw-rw-r--   0 root         (0)     1003    14660 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/context/attribute_context_pb2.py
--rw-rw-r--   0 root         (0)     1003     1861 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/context/audit_context.proto
--rw-rw-r--   0 root         (0)     1003     2603 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/context/audit_context_pb2.py
--rw-rw-r--   0 root         (0)     1003    10869 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/error_details.proto
--rw-rw-r--   0 root         (0)     1003    11094 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/error_details_pb2.py
--rw-rw-r--   0 root         (0)     1003     1940 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/http.proto
--rw-rw-r--   0 root         (0)     1003     3404 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/http_pb2.py
--rw-rw-r--   0 root         (0)     1003     1934 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/status.proto
--rw-rw-r--   0 root         (0)     1003     2302 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/rpc/status_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.641857 googleapis-common-protos-1.63.0/google/type/
--rw-rw-r--   0 root         (0)     1003     1762 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/calendar_period.proto
--rw-rw-r--   0 root         (0)     1003     2343 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/calendar_period_pb2.py
--rw-rw-r--   0 root         (0)     1003     6376 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/color.proto
--rw-rw-r--   0 root         (0)     1003     2343 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/color_pb2.py
--rw-rw-r--   0 root         (0)     1003     1955 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/date.proto
--rw-rw-r--   0 root         (0)     1003     2138 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/date_pb2.py
--rw-rw-r--   0 root         (0)     1003     3905 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/datetime.proto
--rw-rw-r--   0 root         (0)     1003     3165 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/datetime_pb2.py
--rw-rw-r--   0 root         (0)     1003     1204 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/dayofweek.proto
--rw-rw-r--   0 root         (0)     1003     2278 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/dayofweek_pb2.py
--rw-rw-r--   0 root         (0)     1003     4213 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/decimal.proto
--rw-rw-r--   0 root         (0)     1003     2132 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/decimal_pb2.py
--rw-rw-r--   0 root         (0)     1003     2730 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/expr.proto
--rw-rw-r--   0 root         (0)     1003     2153 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/expr_pb2.py
--rw-rw-r--   0 root         (0)     1003     1156 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/fraction.proto
--rw-rw-r--   0 root         (0)     1003     2166 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/fraction_pb2.py
--rw-rw-r--   0 root         (0)     1003     1667 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/interval.proto
--rw-rw-r--   0 root         (0)     1003     2364 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/interval_pb2.py
--rw-rw-r--   0 root         (0)     1003     1447 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/latlng.proto
--rw-rw-r--   0 root         (0)     1003     2144 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/latlng_pb2.py
--rw-rw-r--   0 root         (0)     1003     1303 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/localized_text.proto
--rw-rw-r--   0 root         (0)     1003     2270 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/localized_text_pb2.py
--rw-rw-r--   0 root         (0)     1003     1603 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/money.proto
--rw-rw-r--   0 root         (0)     1003     2151 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/money_pb2.py
--rw-rw-r--   0 root         (0)     1003     1479 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/month.proto
--rw-rw-r--   0 root         (0)     1003     2398 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/month_pb2.py
--rw-rw-r--   0 root         (0)     1003     4744 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/phone_number.proto
--rw-rw-r--   0 root         (0)     1003     3046 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/phone_number_pb2.py
--rw-rw-r--   0 root         (0)     1003     6235 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/postal_address.proto
--rw-rw-r--   0 root         (0)     1003     2654 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/postal_address_pb2.py
--rw-rw-r--   0 root         (0)     1003     3791 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/quaternion.proto
--rw-rw-r--   0 root         (0)     1003     2261 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/quaternion_pb2.py
--rw-rw-r--   0 root         (0)     1003     1667 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/timeofday.proto
--rw-rw-r--   0 root         (0)     1003     2266 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/google/type/timeofday_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.641857 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/
--rw-r--r--   0 root         (0)     1003     1529 2024-03-11 12:33:12.000000 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4150 2024-03-11 12:33:12.000000 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-11 12:33:12.000000 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003      127 2024-03-11 12:33:12.000000 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-11 12:33:12.000000 googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-03-11 12:33:12.645857 googleapis-common-protos-1.63.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2409 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.609855 googleapis-common-protos-1.63.0/tests/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-11 12:33:12.645857 googleapis-common-protos-1.63.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      663 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/tests/unit/test_google_api_error_reason.py
--rw-rw-r--   0 root         (0)     1003     1870 2024-03-11 12:30:49.000000 googleapis-common-protos-1.63.0/tests/unit/test_packaging.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.363110 googleapis-common-protos-1.63.1rc0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     1532 2024-05-30 18:44:32.363110 googleapis-common-protos-1.63.1rc0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003      362 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.327109 googleapis-common-protos-1.63.1rc0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.343110 googleapis-common-protos-1.63.1rc0/google/api/
+-rw-rw-r--   0 root         (0)     1003     1045 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/annotations.proto
+-rw-rw-r--   0 root         (0)     1003     2133 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/annotations_pb2.py
+-rw-rw-r--   0 root         (0)     1003     9257 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/auth.proto
+-rw-rw-r--   0 root         (0)     1003     5613 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/auth_pb2.py
+-rw-rw-r--   0 root         (0)     1003     7014 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/backend.proto
+-rw-rw-r--   0 root         (0)     1003     4838 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/backend_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3062 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/billing.proto
+-rw-rw-r--   0 root         (0)     1003     2933 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/billing_pb2.py
+-rw-rw-r--   0 root         (0)     1003    14713 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/client.proto
+-rw-rw-r--   0 root         (0)     1003    17267 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/client_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3166 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/config_change.proto
+-rw-rw-r--   0 root         (0)     1003     3374 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/config_change_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2717 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/consumer.proto
+-rw-rw-r--   0 root         (0)     1003     3138 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/consumer_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3067 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/context.proto
+-rw-rw-r--   0 root         (0)     1003     2844 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/context_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1436 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/control.proto
+-rw-rw-r--   0 root         (0)     1003     2300 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/control_pb2.py
+-rw-rw-r--   0 root         (0)     1003     8660 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/distribution.proto
+-rw-rw-r--   0 root         (0)     1003     7845 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/distribution_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6940 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/documentation.proto
+-rw-rw-r--   0 root         (0)     1003     3698 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/documentation_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3028 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/endpoint.proto
+-rw-rw-r--   0 root         (0)     1003     2380 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/endpoint_pb2.py
+-rw-rw-r--   0 root         (0)     1003    22644 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/error_reason.proto
+-rw-rw-r--   0 root         (0)     1003     4267 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/error_reason_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4306 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/field_behavior.proto
+-rw-rw-r--   0 root         (0)     1003     2973 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/field_behavior_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3156 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/field_info.proto
+-rw-rw-r--   0 root         (0)     1003     2920 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/field_info_pb2.py
+-rw-rw-r--   0 root         (0)     1003    15159 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/http.proto
+-rw-rw-r--   0 root         (0)     1003     3701 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/http_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2693 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/httpbody.proto
+-rw-rw-r--   0 root         (0)     1003     2344 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/httpbody_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1389 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/label.proto
+-rw-rw-r--   0 root         (0)     1003     2581 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/label_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3083 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/launch_stage.proto
+-rw-rw-r--   0 root         (0)     1003     2277 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/launch_stage_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2043 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/log.proto
+-rw-rw-r--   0 root         (0)     1003     2402 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/log_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3174 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/logging.proto
+-rw-rw-r--   0 root         (0)     1003     3014 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/logging_pb2.py
+-rw-rw-r--   0 root         (0)     1003    10605 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/metric.proto
+-rw-rw-r--   0 root         (0)     1003     6432 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/metric_pb2.py
+-rw-rw-r--   0 root         (0)     1003     5920 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/monitored_resource.proto
+-rw-rw-r--   0 root         (0)     1003     6324 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/monitored_resource_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4457 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/monitoring.proto
+-rw-rw-r--   0 root         (0)     1003     3129 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/monitoring_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3254 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/policy.proto
+-rw-rw-r--   0 root         (0)     1003     3608 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/policy_pb2.py
+-rw-rw-r--   0 root         (0)     1003     7138 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/quota.proto
+-rw-rw-r--   0 root         (0)     1003     5303 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/quota_pb2.py
+-rw-rw-r--   0 root         (0)     1003     8744 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/resource.proto
+-rw-rw-r--   0 root         (0)     1003     4870 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/resource_pb2.py
+-rw-rw-r--   0 root         (0)     1003    14929 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/routing.proto
+-rw-rw-r--   0 root         (0)     1003     3189 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/routing_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6762 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/service.proto
+-rw-rw-r--   0 root         (0)     1003     5979 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/service_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1091 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/source_info.proto
+-rw-rw-r--   0 root         (0)     1003     2292 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/source_info_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3475 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/system_parameter.proto
+-rw-rw-r--   0 root         (0)     1003     3583 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/system_parameter_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3787 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/usage.proto
+-rw-rw-r--   0 root         (0)     1003     2791 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/usage_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3799 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/visibility.proto
+-rw-rw-r--   0 root         (0)     1003     4956 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/api/visibility_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.343110 googleapis-common-protos-1.63.1rc0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003     6307 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/cloud/extended_operations.proto
+-rw-rw-r--   0 root         (0)     1003     4032 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/cloud/extended_operations_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.343110 googleapis-common-protos-1.63.1rc0/google/cloud/location/
+-rw-rw-r--   0 root         (0)     1003     3604 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/cloud/location/locations.proto
+-rw-rw-r--   0 root         (0)     1003     6899 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/cloud/location/locations_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.323109 googleapis-common-protos-1.63.1rc0/google/gapic/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.347110 googleapis-common-protos-1.63.1rc0/google/gapic/metadata/
+-rw-rw-r--   0 root         (0)     1003     3393 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/gapic/metadata/gapic_metadata.proto
+-rw-rw-r--   0 root         (0)     1003     8346 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/gapic/metadata/gapic_metadata_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.323109 googleapis-common-protos-1.63.1rc0/google/logging/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.347110 googleapis-common-protos-1.63.1rc0/google/logging/type/
+-rw-rw-r--   0 root         (0)     1003     3601 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/logging/type/http_request.proto
+-rw-rw-r--   0 root         (0)     1003     3176 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/logging/type/http_request_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2555 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/logging/type/log_severity.proto
+-rw-rw-r--   0 root         (0)     1003     2622 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/logging/type/log_severity_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.347110 googleapis-common-protos-1.63.1rc0/google/longrunning/
+-rw-rw-r--   0 root         (0)     1003    10513 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations.proto
+-rw-rw-r--   0 root         (0)     1003      797 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_grpc.py
+-rw-rw-r--   0 root         (0)     1003      914 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_grpc_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2253 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_pb2.py
+-rw-rw-r--   0 root         (0)     1003    14464 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0)     1003      222 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_proto.py
+-rw-rw-r--   0 root         (0)     1003    10443 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/longrunning/operations_proto_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.351110 googleapis-common-protos-1.63.1rc0/google/rpc/
+-rw-rw-r--   0 root         (0)     1003     7138 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/code.proto
+-rw-rw-r--   0 root         (0)     1003     2707 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/code_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.351110 googleapis-common-protos-1.63.1rc0/google/rpc/context/
+-rw-rw-r--   0 root         (0)     1003    14852 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/context/attribute_context.proto
+-rw-rw-r--   0 root         (0)     1003    14660 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/context/attribute_context_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1861 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/context/audit_context.proto
+-rw-rw-r--   0 root         (0)     1003     2603 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/context/audit_context_pb2.py
+-rw-rw-r--   0 root         (0)     1003    10869 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/error_details.proto
+-rw-rw-r--   0 root         (0)     1003    11094 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/error_details_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1940 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/http.proto
+-rw-rw-r--   0 root         (0)     1003     3404 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/http_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1934 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/status.proto
+-rw-rw-r--   0 root         (0)     1003     2302 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/rpc/status_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.359110 googleapis-common-protos-1.63.1rc0/google/type/
+-rw-rw-r--   0 root         (0)     1003     1762 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/calendar_period.proto
+-rw-rw-r--   0 root         (0)     1003     2343 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/calendar_period_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6376 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/color.proto
+-rw-rw-r--   0 root         (0)     1003     2343 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/color_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1955 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/date.proto
+-rw-rw-r--   0 root         (0)     1003     2138 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/date_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3905 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/datetime.proto
+-rw-rw-r--   0 root         (0)     1003     3165 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/datetime_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1204 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/dayofweek.proto
+-rw-rw-r--   0 root         (0)     1003     2278 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/dayofweek_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4213 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/decimal.proto
+-rw-rw-r--   0 root         (0)     1003     2132 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/decimal_pb2.py
+-rw-rw-r--   0 root         (0)     1003     2730 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/expr.proto
+-rw-rw-r--   0 root         (0)     1003     2153 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/expr_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1156 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/fraction.proto
+-rw-rw-r--   0 root         (0)     1003     2166 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/fraction_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1667 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/interval.proto
+-rw-rw-r--   0 root         (0)     1003     2364 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/interval_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1447 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/latlng.proto
+-rw-rw-r--   0 root         (0)     1003     2144 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/latlng_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1303 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/localized_text.proto
+-rw-rw-r--   0 root         (0)     1003     2270 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/localized_text_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1603 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/money.proto
+-rw-rw-r--   0 root         (0)     1003     2151 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/money_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1479 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/month.proto
+-rw-rw-r--   0 root         (0)     1003     2398 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/month_pb2.py
+-rw-rw-r--   0 root         (0)     1003     4744 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/phone_number.proto
+-rw-rw-r--   0 root         (0)     1003     3046 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/phone_number_pb2.py
+-rw-rw-r--   0 root         (0)     1003     6235 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/postal_address.proto
+-rw-rw-r--   0 root         (0)     1003     2654 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/postal_address_pb2.py
+-rw-rw-r--   0 root         (0)     1003     3791 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/quaternion.proto
+-rw-rw-r--   0 root         (0)     1003     2261 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/quaternion_pb2.py
+-rw-rw-r--   0 root         (0)     1003     1667 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/timeofday.proto
+-rw-rw-r--   0 root         (0)     1003     2266 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/google/type/timeofday_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.363110 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/
+-rw-r--r--   0 root         (0)     1003     1532 2024-05-30 18:44:32.000000 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4150 2024-05-30 18:44:32.000000 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-30 18:44:32.000000 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003      127 2024-05-30 18:44:32.000000 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-30 18:44:32.000000 googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-05-30 18:44:32.363110 googleapis-common-protos-1.63.1rc0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2412 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.327109 googleapis-common-protos-1.63.1rc0/tests/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-30 18:44:32.359110 googleapis-common-protos-1.63.1rc0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      663 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/tests/unit/test_google_api_error_reason.py
+-rw-rw-r--   0 root         (0)     1003     1870 2024-05-30 18:41:46.000000 googleapis-common-protos-1.63.1rc0/tests/unit/test_packaging.py
```

### Comparing `googleapis-common-protos-1.63.0/LICENSE` & `googleapis-common-protos-1.63.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/MANIFEST.in` & `googleapis-common-protos-1.63.1rc0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/PKG-INFO` & `googleapis-common-protos-1.63.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.63.0
+Version: 1.63.1rc0
 Summary: Common protobufs used in Google APIs
 Home-page: https://github.com/googleapis/python-api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0.dev0,>=3.19.5
+Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<6.0.0.dev0,>=3.19.5
 Provides-Extra: grpc
 Requires-Dist: grpcio<2.0.0.dev0,>=1.44.0; extra == "grpc"
 
 Google APIs common protos
 -------------------------
 
 .. image:: https://img.shields.io/pypi/v/googleapis-common-protos.svg
```

### Comparing `googleapis-common-protos-1.63.0/google/api/annotations.proto` & `googleapis-common-protos-1.63.1rc0/google/api/annotations.proto`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2015 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/annotations_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/annotations_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/auth.proto` & `googleapis-common-protos-1.63.1rc0/google/api/auth.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/auth_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/auth_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/backend.proto` & `googleapis-common-protos-1.63.1rc0/google/api/backend.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/backend_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/backend_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/billing.proto` & `googleapis-common-protos-1.63.1rc0/google/api/billing.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/billing_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/billing_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/client.proto` & `googleapis-common-protos-1.63.1rc0/google/api/client.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/client_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/client_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/config_change.proto` & `googleapis-common-protos-1.63.1rc0/google/api/config_change.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/config_change_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/config_change_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/consumer.proto` & `googleapis-common-protos-1.63.1rc0/google/api/consumer.proto`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2016 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/consumer_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/consumer_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/context.proto` & `googleapis-common-protos-1.63.1rc0/google/api/context.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/context_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/context_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/control.proto` & `googleapis-common-protos-1.63.1rc0/google/api/control.proto`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/control_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/control_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/distribution.proto` & `googleapis-common-protos-1.63.1rc0/google/api/distribution.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/distribution_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/distribution_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/documentation.proto` & `googleapis-common-protos-1.63.1rc0/google/api/documentation.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/documentation_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/documentation_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/endpoint.proto` & `googleapis-common-protos-1.63.1rc0/google/api/endpoint.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/endpoint_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/endpoint_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/error_reason.proto` & `googleapis-common-protos-1.63.1rc0/google/api/error_reason.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/error_reason_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/error_reason_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/field_behavior.proto` & `googleapis-common-protos-1.63.1rc0/google/api/field_behavior.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/field_behavior_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/field_behavior_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/field_info.proto` & `googleapis-common-protos-1.63.1rc0/google/api/field_info.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/field_info_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/field_info_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/http.proto` & `googleapis-common-protos-1.63.1rc0/google/api/http.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/http_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/http_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/httpbody.proto` & `googleapis-common-protos-1.63.1rc0/google/api/httpbody.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/httpbody_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/httpbody_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/label.proto` & `googleapis-common-protos-1.63.1rc0/google/api/label.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/label_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/label_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/launch_stage.proto` & `googleapis-common-protos-1.63.1rc0/google/api/launch_stage.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/launch_stage_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/launch_stage_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/log.proto` & `googleapis-common-protos-1.63.1rc0/google/api/log.proto`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/log_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/log_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/logging.proto` & `googleapis-common-protos-1.63.1rc0/google/api/logging.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/logging_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/logging_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/metric.proto` & `googleapis-common-protos-1.63.1rc0/google/api/metric.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/metric_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/metric_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/monitored_resource.proto` & `googleapis-common-protos-1.63.1rc0/google/api/monitored_resource.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/monitored_resource_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/monitored_resource_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/monitoring.proto` & `googleapis-common-protos-1.63.1rc0/google/api/monitoring.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/monitoring_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/monitoring_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/policy.proto` & `googleapis-common-protos-1.63.1rc0/google/api/policy.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/policy_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/policy_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/quota.proto` & `googleapis-common-protos-1.63.1rc0/google/api/quota.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/quota_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/quota_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/resource.proto` & `googleapis-common-protos-1.63.1rc0/google/api/resource.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/resource_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/resource_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/routing.proto` & `googleapis-common-protos-1.63.1rc0/google/api/routing.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC // // Licensed under the Apache License, Version
+// Copyright 2024 Google LLC // // Licensed under the Apache License, Version
 2.0 (the "License"); // you may not use this file except in compliance with the
 License. // You may obtain a copy of the License at // // http://
 www.apache.org/licenses/LICENSE-2.0 // // Unless required by applicable law or
 agreed to in writing, software // distributed under the License is distributed
 on an "AS IS" BASIS, // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. // See the License for the specific language governing
 permissions and // limitations under the License. syntax = "proto3"; package
```

### Comparing `googleapis-common-protos-1.63.0/google/api/routing_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/routing_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/service.proto` & `googleapis-common-protos-1.63.1rc0/google/api/service.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/service_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/source_info.proto` & `googleapis-common-protos-1.63.1rc0/google/api/source_info.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/source_info_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/source_info_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/system_parameter.proto` & `googleapis-common-protos-1.63.1rc0/google/api/system_parameter.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/system_parameter_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/system_parameter_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/usage.proto` & `googleapis-common-protos-1.63.1rc0/google/api/usage.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/usage_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/usage_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/api/visibility.proto` & `googleapis-common-protos-1.63.1rc0/google/api/visibility.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/api/visibility_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/api/visibility_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/cloud/extended_operations.proto` & `googleapis-common-protos-1.63.1rc0/google/cloud/extended_operations.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC.
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/cloud/extended_operations_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/cloud/extended_operations_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/cloud/location/locations.proto` & `googleapis-common-protos-1.63.1rc0/google/cloud/location/locations.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2020 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/cloud/location/locations_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/cloud/location/locations_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/gapic/metadata/gapic_metadata.proto` & `googleapis-common-protos-1.63.1rc0/google/gapic/metadata/gapic_metadata.proto`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 option go_package = "google.golang.org/genproto/googleapis/gapic/metadata;metadata";
 option java_multiple_files = true;
 option java_outer_classname = "GapicMetadataProto";
 option java_package = "com.google.gapic.metadata";
 option php_namespace = "Google\\Gapic\\Metadata";
 option ruby_package = "Google::Gapic::Metadata";
 
-// Metadata about a GAPIC library for a specific combination of API, version, and
-// computer language.
+// Metadata about a GAPIC library for a specific combination of API, version,
+// and computer language.
 message GapicMetadata {
   // Schema version of this proto. Current value: 1.0
   string schema = 1;
 
   // Any human-readable comments to be included in this file.
   string comment = 2;
 
@@ -70,23 +70,22 @@
     string library_client = 1;
 
     // A mapping from each proto-defined RPC name to the the list of
     // methods in library_client that implement it. There can be more
     // than one library_client method for each RPC. RPCs with no
     // library_client methods need not be included.
     //
-    // The key name is the name of the RPC as defined and formated in
+    // The key name is the name of the RPC as defined and formatted in
     // the proto file.
     map<string, MethodList> rpcs = 2;
   }
 
   // List of GAPIC client methods implementing the proto-defined RPC
   // for the transport and service specified in the containing
   // structures.
   message MethodList {
     // List of methods for a specific proto-service client in the
     // GAPIC. These names should be formatted as they appear in the
     // source code.
     repeated string methods = 1;
   }
-
 }
```

### Comparing `googleapis-common-protos-1.63.0/google/gapic/metadata/gapic_metadata_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/gapic/metadata/gapic_metadata_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/logging/type/http_request.proto` & `googleapis-common-protos-1.63.1rc0/google/logging/type/http_request.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/logging/type/http_request_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/logging/type/http_request_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/logging/type/log_severity.proto` & `googleapis-common-protos-1.63.1rc0/google/logging/type/log_severity.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2023 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/logging/type/log_severity_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/logging/type/log_severity_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations.proto` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2020 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations_grpc.py` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations_grpc.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations_grpc_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations_pb2_grpc.py` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/google/longrunning/operations_proto_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/longrunning/operations_proto_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/code.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/code.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/code_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/code_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/context/attribute_context.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/context/attribute_context.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/context/attribute_context_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/context/attribute_context_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/context/audit_context.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/context/audit_context.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/context/audit_context_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/context/audit_context_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/error_details.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/error_details.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/error_details_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/error_details_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/http.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/http.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/http_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/http_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/status.proto` & `googleapis-common-protos-1.63.1rc0/google/rpc/status.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2022 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/rpc/status_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/rpc/status_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/calendar_period.proto` & `googleapis-common-protos-1.63.1rc0/google/type/calendar_period.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/calendar_period_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/calendar_period_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/color.proto` & `googleapis-common-protos-1.63.1rc0/google/type/color.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/color_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/color_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/date.proto` & `googleapis-common-protos-1.63.1rc0/google/type/date.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/date_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/date_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/datetime.proto` & `googleapis-common-protos-1.63.1rc0/google/type/datetime.proto`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/datetime_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/datetime_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/dayofweek.proto` & `googleapis-common-protos-1.63.1rc0/google/type/dayofweek.proto`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/dayofweek_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/dayofweek_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/decimal.proto` & `googleapis-common-protos-1.63.1rc0/google/type/decimal.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/decimal_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/decimal_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/expr.proto` & `googleapis-common-protos-1.63.1rc0/google/type/expr.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/expr_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/expr_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/fraction.proto` & `googleapis-common-protos-1.63.1rc0/google/type/fraction.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/fraction_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/fraction_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/interval.proto` & `googleapis-common-protos-1.63.1rc0/google/type/interval.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/interval_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/interval_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/latlng.proto` & `googleapis-common-protos-1.63.1rc0/google/type/latlng.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC // // Licensed under the Apache License, Version
+// Copyright 2024 Google LLC // // Licensed under the Apache License, Version
 2.0 (the "License"); // you may not use this file except in compliance with the
 License. // You may obtain a copy of the License at // // http://
 www.apache.org/licenses/LICENSE-2.0 // // Unless required by applicable law or
 agreed to in writing, software // distributed under the License is distributed
 on an "AS IS" BASIS, // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 express or implied. // See the License for the specific language governing
 permissions and // limitations under the License. syntax = "proto3"; package
```

### Comparing `googleapis-common-protos-1.63.0/google/type/latlng_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/latlng_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/localized_text.proto` & `googleapis-common-protos-1.63.1rc0/google/type/localized_text.proto`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/localized_text_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/localized_text_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/money.proto` & `googleapis-common-protos-1.63.1rc0/google/type/money.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/money_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/money_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/month.proto` & `googleapis-common-protos-1.63.1rc0/google/type/month.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/month_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/month_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/phone_number.proto` & `googleapis-common-protos-1.63.1rc0/google/type/phone_number.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/phone_number_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/phone_number_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/postal_address.proto` & `googleapis-common-protos-1.63.1rc0/google/type/postal_address.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/postal_address_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/postal_address_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/quaternion.proto` & `googleapis-common-protos-1.63.1rc0/google/type/quaternion.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/quaternion_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/quaternion_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/google/type/timeofday.proto` & `googleapis-common-protos-1.63.1rc0/google/type/timeofday.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2024 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `googleapis-common-protos-1.63.0/google/type/timeofday_pb2.py` & `googleapis-common-protos-1.63.1rc0/google/type/timeofday_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2020 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/PKG-INFO` & `googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapis-common-protos
-Version: 1.63.0
+Version: 1.63.1rc0
 Summary: Common protobufs used in Google APIs
 Home-page: https://github.com/googleapis/python-api-common-protos
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0.dev0,>=3.19.5
+Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<6.0.0.dev0,>=3.19.5
 Provides-Extra: grpc
 Requires-Dist: grpcio<2.0.0.dev0,>=1.44.0; extra == "grpc"
 
 Google APIs common protos
 -------------------------
 
 .. image:: https://img.shields.io/pypi/v/googleapis-common-protos.svg
```

### Comparing `googleapis-common-protos-1.63.0/googleapis_common_protos.egg-info/SOURCES.txt` & `googleapis-common-protos-1.63.1rc0/googleapis_common_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/setup.py` & `googleapis-common-protos-1.63.1rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 import setuptools
 from setuptools import find_namespace_packages
 
 
 name = "googleapis-common-protos"
 description = "Common protobufs used in Google APIs"
-version = "1.63.0"
+version = "1.63.1rc0"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
-    "protobuf>=3.19.5,<5.0.0.dev0,!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+    "protobuf>=3.19.5,<6.0.0.dev0,!=3.20.0,!=3.20.1,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 
 extras_require = {"grpc": ["grpcio >= 1.44.0, <2.0.0.dev0"]}
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
```

### Comparing `googleapis-common-protos-1.63.0/tests/unit/test_google_api_error_reason.py` & `googleapis-common-protos-1.63.1rc0/tests/unit/test_google_api_error_reason.py`

 * *Files identical despite different names*

### Comparing `googleapis-common-protos-1.63.0/tests/unit/test_packaging.py` & `googleapis-common-protos-1.63.1rc0/tests/unit/test_packaging.py`

 * *Files identical despite different names*

