# Comparing `tmp/layrz_sdk-3.0.2.tar.gz` & `tmp/layrz_sdk-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz_sdk-3.0.2.tar", last modified: Mon May 13 14:50:15 2024, max compression
+gzip compressed data, was "layrz_sdk-3.0.3.tar", last modified: Thu May 30 00:00:13 2024, max compression
```

## Comparing `layrz_sdk-3.0.2.tar` & `layrz_sdk-3.0.3.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/
--rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      628 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/entities/
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      566 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/request.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/response.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/result.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/service.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.315596 layrz_sdk-3.0.2/layrz_sdk/entities/cases/
--rw-rw-r--   0 root         (0) root         (0)      135 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/case.py
--rw-rw-r--   0 root         (0) root         (0)      902 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/comment.py
--rw-rw-r--   0 root         (0) root         (0)      629 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.315596 layrz_sdk-3.0.2/layrz_sdk/entities/charts/
--rw-rw-r--   0 root         (0) root         (0)      753 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      438 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/alignment.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/bar.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/column.py
--rw-rw-r--   0 root         (0) root         (0)      514 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/configuration.py
--rw-rw-r--   0 root         (0) root         (0)      447 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/data_type.py
--rw-rw-r--   0 root         (0) root         (0)      558 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      995 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/html.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/line.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/map.py
--rw-rw-r--   0 root         (0) root         (0)      811 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/number.py
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/pie.py
--rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/radar.py
--rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/radial_bar.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/scatter.py
--rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie.py
--rw-rw-r--   0 root         (0) root         (0)      463 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie_type.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/table.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/
--rw-rw-r--   0 root         (0) root         (0)      126 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)      653 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/geofence.py
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/events/
--rw-rw-r--   0 root         (0) root         (0)       49 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/events/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      467 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/general/
--rw-rw-r--   0 root         (0) root         (0)      218 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/asset.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/asset_operation_mode.py
--rw-rw-r--   0 root         (0) root         (0)      606 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/custom_field.py
--rw-rw-r--   0 root         (0) root         (0)      973 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/device.py
--rw-rw-r--   0 root         (0) root         (0)      615 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/sensor.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/entities/reports/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/col.py
--rw-rw-r--   0 root         (0) root         (0)      442 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/format.py
--rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/header.py
--rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/page.py
--rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/report.py
--rw-rw-r--   0 root         (0) root         (0)      881 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      789 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/message.py
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/helpers/
--rw-rw-r--   0 root         (0) root         (0)       72 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/lcl/
--rw-rw-r--   0 root         (0) root         (0)       67 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/lcl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22987 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/tests/
--rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/tests/test_lcl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/
+-rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.778777 layrz_sdk-3.0.3/layrz_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.782777 layrz_sdk-3.0.3/layrz_sdk/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1350 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.782777 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/request.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/response.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/result.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/service.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.782777 layrz_sdk-3.0.3/layrz_sdk/entities/cases/
+-rw-rw-r--   0 root         (0) root         (0)      135 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/cases/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/cases/case.py
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/cases/comment.py
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.786777 layrz_sdk-3.0.3/layrz_sdk/entities/charts/
+-rw-rw-r--   0 root         (0) root         (0)      806 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/alignment.py
+-rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/column.py
+-rw-rw-r--   0 root         (0) root         (0)      514 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)      447 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/data_type.py
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/html.py
+-rw-rw-r--   0 root         (0) root         (0)     6586 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/line.py
+-rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/map.py
+-rw-rw-r--   0 root         (0) root         (0)      811 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/number.py
+-rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/pie.py
+-rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/radar.py
+-rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/radial_bar.py
+-rw-rw-r--   0 root         (0) root         (0)      524 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/render_technology.py
+-rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/scatter.py
+-rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/serie.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/serie_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/table.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.786777 layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/checkpoint.py
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/geofence.py
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.790777 layrz_sdk-3.0.3/layrz_sdk/entities/events/
+-rw-rw-r--   0 root         (0) root         (0)       49 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/events/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.790777 layrz_sdk-3.0.3/layrz_sdk/entities/formatting/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/formatting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.790777 layrz_sdk-3.0.3/layrz_sdk/entities/general/
+-rw-rw-r--   0 root         (0) root         (0)      218 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/asset.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/asset_operation_mode.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/custom_field.py
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/device.py
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/sensor.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.790777 layrz_sdk-3.0.3/layrz_sdk/entities/repcom/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/repcom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/layrz_sdk/entities/reports/
+-rw-rw-r--   0 root         (0) root         (0)      249 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/col.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/format.py
+-rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/header.py
+-rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/page.py
+-rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/report.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/message.py
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/layrz_sdk/helpers/
+-rw-rw-r--   0 root         (0) root         (0)       72 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/layrz_sdk/lcl/
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/lcl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22987 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/layrz_sdk/lcl/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-30 00:00:13.000000 layrz_sdk-3.0.3/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2570 2024-05-30 00:00:13.000000 layrz_sdk-3.0.3/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 00:00:13.000000 layrz_sdk-3.0.3/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-30 00:00:13.000000 layrz_sdk-3.0.3/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-30 00:00:13.000000 layrz_sdk-3.0.3/layrz_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 00:00:13.794777 layrz_sdk-3.0.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-29 23:59:19.000000 layrz_sdk-3.0.3/tests/test_lcl.py
```

### Comparing `layrz_sdk-3.0.2/LICENSE` & `layrz_sdk-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/PKG-INFO` & `layrz_sdk-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.2
+Version: 3.0.3
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.2/README.md` & `layrz_sdk-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/__init__.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Init file """
 # Broadcast entities
 from .broadcasts import (BroadcastRequest, BroadcastResponse, BroadcastResult, BroadcastStatus, OutboundService)
 # Cases entitites
 from .cases import Case, CaseIgnoredStatus, CaseStatus, Comment, Trigger
 # Charts entities
 from .charts import (AreaChart, BarChart, ChartAlignment, ChartConfiguration, ChartDataSerie, ChartDataSerieType,
-                     ChartDataType, ChartException, ColumnChart, HTMLChart, LineChart, MapCenterType, MapChart,
-                     MapPoint, NumberChart, PieChart, RadarChart, RadialBarChart, ScatterChart, ScatterSerie,
-                     ScatterSerieItem, TableChart, TableHeader, TableRow, TimelineChart, TimelineSerie,
+                     ChartDataType, ChartException, ChartRenderTechnology, ColumnChart, HTMLChart, LineChart,
+                     MapCenterType, MapChart, MapPoint, NumberChart, PieChart, RadarChart, RadialBarChart, ScatterChart,
+                     ScatterSerie, ScatterSerieItem, TableChart, TableHeader, TableRow, TimelineChart, TimelineSerie,
                      TimelineSerieItem)
 # Checkpoints entities
 from .checkpoints import Checkpoint, Geofence, Waypoint
 # Events entities
 from .events import Event
 # Formatting entities
 from .formatting import TextAlignment
```

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/request.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/request.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/response.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/response.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/result.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/result.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/service.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/service.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/status.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/broadcasts/status.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/cases/case.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/cases/case.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/cases/comment.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/cases/comment.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/cases/trigger.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/cases/trigger.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/__init__.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 from .html import HTMLChart
 from .line import AreaChart, LineChart
 from .map import MapCenterType, MapChart, MapPoint
 from .number import NumberChart
 from .pie import PieChart
 from .radar import RadarChart
 from .radial_bar import RadialBarChart
+from .render_technology import ChartRenderTechnology
 from .scatter import ScatterChart, ScatterSerie, ScatterSerieItem
 from .serie import ChartDataSerie
 from .serie_type import ChartDataSerieType
 from .table import TableChart, TableHeader, TableRow
 from .timeline import TimelineChart, TimelineSerie, TimelineSerieItem
```

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/bar.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/column.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/column.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/configuration.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/configuration.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/exceptions.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/html.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/html.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/line.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/line.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Line chart """
 
 from .alignment import ChartAlignment
 from .data_type import ChartDataType
 from .exceptions import ChartException
+from .render_technology import ChartRenderTechnology
 from .serie import ChartDataSerie
 from .serie_type import ChartDataSerieType
 
 
 class LineChart:
   """
   Line chart configuration
@@ -44,35 +45,84 @@
       raise ChartException('title must be an instance of str')
     self.title = title
 
     if not isinstance(align, ChartAlignment):
       raise ChartException('align must be an instance of ChartAlignment')
     self.align = align
 
-  def render(self, use_new_definition: bool = False) -> dict | list[dict]:
+  def render(self, technology: ChartRenderTechnology) -> dict | list[dict]:
     """
     Render chart to a graphic Library.
     We have two graphic libraries: GRAPHIC and CANVASJS.
 
     GRAPHIC is a Flutter chart library. To return this option, use the parameter use_new_definition=True.
     CANVASJS is a Javascript chart library. This is the default option.
     """
 
-    if use_new_definition:
+    if technology == ChartRenderTechnology.GRAPHIC:
       return {
         'library': 'GRAPHIC',
         'chart': 'LINE',
         'configuration': self._render_graphic(),
       }
+
+    if technology == ChartRenderTechnology.SYNCFUSION_FLUTTER_CHARTS:
+      return {
+        'library': 'syncfusion_flutter_charts',
+        'chart': 'LINE',
+        'configuration': self._render_syncfusion_flutter_charts(),
+      }
+
     return {
       'library': 'CANVASJS',
       'chart': 'LINE',
       'configuration': self._render_canvasjs(),
     }
 
+  def _render_syncfusion_flutter_charts(self) -> list[dict]:
+    """ 
+    Converts the configuration of the chart to a Flutter library syncfusion_flutter_charts.
+    """
+    series = []
+
+    for serie in self.y_axis:
+      if serie.serie_type not in [ChartDataSerieType.LINE, ChartDataSerieType.AREA]:
+        continue
+
+      points = []
+
+      for i, value in enumerate(self.x_axis.data):
+        x_value = value.timestamp() if self.x_axis.data_type == ChartDataType.DATETIME else value
+        if not isinstance(x_value, (int, float)):
+          continue
+
+        y_value = serie.data[i]
+        if isinstance(y_value, bool):
+          if y_value:
+            y_value = 1
+          else:
+            y_value = 0
+
+        if not isinstance(y_value, (int, float)):
+          continue
+
+        points.append({
+          'xAxis': x_value,
+          'yAxis': y_value,
+        })
+
+      series.append({
+        'color': serie.color,
+        'values': points,
+        'label': serie.label,
+        'type': 'AREA' if serie.serie_type == ChartDataSerieType.AREA else 'LINE',
+      })
+
+    return series
+
   def _render_graphic(self) -> list[dict]:
     """
     Converts the configuration of the chart to a Flutter library Graphic.
     """
     series = []
 
     for serie in self.y_axis:
```

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/map.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/map.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/number.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/number.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/pie.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/pie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/radar.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/radar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/radial_bar.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/radial_bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/scatter.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/scatter.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/serie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/table.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/table.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/charts/timeline.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/charts/timeline.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/checkpoint.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/checkpoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/geofence.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/geofence.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/waypoint.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/checkpoints/waypoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/events/event.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/events/event.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/asset.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/asset.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/asset_operation_mode.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/asset_operation_mode.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/custom_field.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/custom_field.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/device.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/device.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/sensor.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/sensor.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/general/user.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/general/user.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/repcom/transaction.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/repcom/transaction.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/reports/col.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/reports/col.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/reports/header.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/reports/header.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/reports/page.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/reports/page.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/reports/report.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/reports/report.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/reports/row.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/reports/row.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/message.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/message.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/position.py` & `layrz_sdk-3.0.3/layrz_sdk/entities/telemetry/position.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/helpers/color.py` & `layrz_sdk-3.0.3/layrz_sdk/helpers/color.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk/lcl/core.py` & `layrz_sdk-3.0.3/layrz_sdk/lcl/core.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.2/layrz_sdk.egg-info/PKG-INFO` & `layrz_sdk-3.0.3/layrz_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.2
+Version: 3.0.3
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.2/layrz_sdk.egg-info/SOURCES.txt` & `layrz_sdk-3.0.3/layrz_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 layrz_sdk/entities/charts/html.py
 layrz_sdk/entities/charts/line.py
 layrz_sdk/entities/charts/map.py
 layrz_sdk/entities/charts/number.py
 layrz_sdk/entities/charts/pie.py
 layrz_sdk/entities/charts/radar.py
 layrz_sdk/entities/charts/radial_bar.py
+layrz_sdk/entities/charts/render_technology.py
 layrz_sdk/entities/charts/scatter.py
 layrz_sdk/entities/charts/serie.py
 layrz_sdk/entities/charts/serie_type.py
 layrz_sdk/entities/charts/table.py
 layrz_sdk/entities/charts/timeline.py
 layrz_sdk/entities/checkpoints/__init__.py
 layrz_sdk/entities/checkpoints/checkpoint.py
```

### Comparing `layrz_sdk-3.0.2/pyproject.toml` & `layrz_sdk-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "layrz-sdk"
-version = "3.0.2"
+version = "3.0.3"
 description = "Layrz SDK for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
 requires-python = ">=3.10"
 
 maintainers = [
```

### Comparing `layrz_sdk-3.0.2/tests/test_lcl.py` & `layrz_sdk-3.0.3/tests/test_lcl.py`

 * *Files identical despite different names*

