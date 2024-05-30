# Comparing `tmp/datupapi-1.97.0.tar.gz` & `tmp/datupapi-1.97.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datupapi-1.97.0.tar", last modified: Mon May 27 20:54:08 2024, max compression
+gzip compressed data, was "datupapi-1.97.1.tar", last modified: Thu May 30 21:30:45 2024, max compression
```

## Comparing `datupapi-1.97.0.tar` & `datupapi-1.97.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:08.000168 datupapi-1.97.0/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-27 20:54:07.999168 datupapi-1.97.0/PKG-INFO
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.983168 datupapi-1.97.0/datupapi/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.984168 datupapi-1.97.0/datupapi/configure/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/configure/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/configure/config.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.980168 datupapi-1.97.0/datupapi/distribution/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.984168 datupapi-1.97.0/datupapi/distribution/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.0/datupapi/distribution/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.981168 datupapi-1.97.0/datupapi/distribution/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.985168 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.985168 datupapi-1.97.0/datupapi/evaluate/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/evaluate/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.97.0/datupapi/evaluate/errors.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.986168 datupapi-1.97.0/datupapi/extract/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/extract/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    69213 2024-05-21 16:19:09.000000 datupapi-1.97.0/datupapi/extract/io.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.97.0/datupapi/extract/io_citrix.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.987168 datupapi-1.97.0/datupapi/feateng/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/relation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/scale.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.988168 datupapi-1.97.0/datupapi/inventory/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/inventory/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.989168 datupapi-1.97.0/datupapi/inventory/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.982168 datupapi-1.97.0/datupapi/inventory/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.989168 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/daily_usage.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.990168 datupapi-1.97.0/datupapi/inventory/src/Format/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Format/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5822 2024-05-27 20:50:16.000000 datupapi-1.97.0/datupapi/inventory/src/Format/inventory_format.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.990168 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    13036 2024-05-27 20:50:16.000000 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.991168 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/define_periods.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.991168 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.992168 datupapi-1.97.0/datupapi/inventory/src/Transformation/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Transformation/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Transformation/inventory_transformation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/inventory/stocks.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.992168 datupapi-1.97.0/datupapi/predict/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/predict/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/predict/forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.994168 datupapi-1.97.0/datupapi/prepare/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/cleanse.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20792 2024-05-08 23:46:05.000000 datupapi-1.97.0/datupapi/prepare/format.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/format_dask.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.995168 datupapi-1.97.0/datupapi/training/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/attup.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/deepar.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22819 2024-05-08 16:06:10.000000 datupapi-1.97.0/datupapi/training/tft.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.997168 datupapi-1.97.0/datupapi/transform/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/backtesting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    56492 2024-05-08 16:06:10.000000 datupapi-1.97.0/datupapi/transform/forecasting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/ranking.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.997168 datupapi-1.97.0/datupapi/utils/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/utils/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/utils/utils.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.998168 datupapi-1.97.0/datupapi.egg-info/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/PKG-INFO
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/SOURCES.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/dependency_links.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/requires.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/top_level.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.97.0/pyproject.toml
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-05-27 20:54:08.000168 datupapi-1.97.0/setup.cfg
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-05-27 20:52:51.000000 datupapi-1.97.0/setup.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.524527 datupapi-1.97.1/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-30 21:30:45.524527 datupapi-1.97.1/PKG-INFO
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.510527 datupapi-1.97.1/datupapi/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.510527 datupapi-1.97.1/datupapi/configure/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/configure/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/configure/config.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.508527 datupapi-1.97.1/datupapi/distribution/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.511527 datupapi-1.97.1/datupapi/distribution/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.1/datupapi/distribution/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.508527 datupapi-1.97.1/datupapi/distribution/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.511527 datupapi-1.97.1/datupapi/distribution/src/DistributionFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.1/datupapi/distribution/src/DistributionFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.97.1/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.512527 datupapi-1.97.1/datupapi/evaluate/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/evaluate/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.97.1/datupapi/evaluate/errors.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.512527 datupapi-1.97.1/datupapi/extract/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/extract/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    69213 2024-05-21 16:19:09.000000 datupapi-1.97.1/datupapi/extract/io.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.97.1/datupapi/extract/io_citrix.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.513527 datupapi-1.97.1/datupapi/feateng/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/feateng/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/feateng/relation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/feateng/scale.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.514527 datupapi-1.97.1/datupapi/inventory/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/inventory/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.514527 datupapi-1.97.1/datupapi/inventory/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.509527 datupapi-1.97.1/datupapi/inventory/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.515527 datupapi-1.97.1/datupapi/inventory/src/DailyUsage/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/DailyUsage/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/DailyUsage/daily_usage.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.515527 datupapi-1.97.1/datupapi/inventory/src/Format/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/Format/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5822 2024-05-27 20:50:16.000000 datupapi-1.97.1/datupapi/inventory/src/Format/inventory_format.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.516527 datupapi-1.97.1/datupapi/inventory/src/InventoryFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/InventoryFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    13024 2024-05-30 21:30:13.000000 datupapi-1.97.1/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.516527 datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/define_periods.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/extract_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.517527 datupapi-1.97.1/datupapi/inventory/src/SuggestedForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/SuggestedForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.517527 datupapi-1.97.1/datupapi/inventory/src/Transformation/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/Transformation/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.97.1/datupapi/inventory/src/Transformation/inventory_transformation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/inventory/stocks.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.518527 datupapi-1.97.1/datupapi/predict/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/predict/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/predict/forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.519527 datupapi-1.97.1/datupapi/prepare/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/prepare/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/prepare/cleanse.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20792 2024-05-08 23:46:05.000000 datupapi-1.97.1/datupapi/prepare/format.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/prepare/format_dask.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.521527 datupapi-1.97.1/datupapi/training/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/training/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/training/attup.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/training/deepar.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22819 2024-05-08 16:06:10.000000 datupapi-1.97.1/datupapi/training/tft.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.522527 datupapi-1.97.1/datupapi/transform/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/transform/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/transform/backtesting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    56492 2024-05-08 16:06:10.000000 datupapi-1.97.1/datupapi/transform/forecasting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/transform/ranking.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.523527 datupapi-1.97.1/datupapi/utils/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/utils/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.97.1/datupapi/utils/utils.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-30 21:30:45.523527 datupapi-1.97.1/datupapi.egg-info/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-30 21:30:45.000000 datupapi-1.97.1/datupapi.egg-info/PKG-INFO
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-05-30 21:30:45.000000 datupapi-1.97.1/datupapi.egg-info/SOURCES.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-05-30 21:30:45.000000 datupapi-1.97.1/datupapi.egg-info/dependency_links.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-05-30 21:30:45.000000 datupapi-1.97.1/datupapi.egg-info/requires.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-05-30 21:30:45.000000 datupapi-1.97.1/datupapi.egg-info/top_level.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.97.1/pyproject.toml
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-05-30 21:30:45.524527 datupapi-1.97.1/setup.cfg
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-05-30 21:30:13.000000 datupapi-1.97.1/setup.py
```

### Comparing `datupapi-1.97.0/PKG-INFO` & `datupapi-1.97.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.97.0
+Version: 1.97.1
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.97.0/datupapi/configure/config.py` & `datupapi-1.97.1/datupapi/configure/config.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py` & `datupapi-1.97.1/datupapi/distribution/src/DistributionFunctions/functions_distribution.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/evaluate/errors.py` & `datupapi-1.97.1/datupapi/evaluate/errors.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/extract/io.py` & `datupapi-1.97.1/datupapi/extract/io.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/extract/io_citrix.py` & `datupapi-1.97.1/datupapi/extract/io_citrix.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/feateng/relation.py` & `datupapi-1.97.1/datupapi/feateng/relation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/feateng/scale.py` & `datupapi-1.97.1/datupapi/feateng/scale.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/DailyUsage/daily_usage.py` & `datupapi-1.97.1/datupapi/inventory/src/DailyUsage/daily_usage.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/Format/inventory_format.py` & `datupapi-1.97.1/datupapi/inventory/src/Format/inventory_format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py` & `datupapi-1.97.1/datupapi/inventory/src/InventoryFunctions/functions_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                 ) else x['ReorderStatus'], axis=1
             )
 
             df['ReorderStatus'] = df.apply(
                 lambda x: 'Order' if (
                     x['ReorderStatus'] == 'Order' and 
                     (x['InvTransStockoutDays'] <= x['AvgLeadTime'] or x['OrderDays'] == 0)
-                ) else x['ReorderStatus'], axis=1
+                ) else 'Hold', axis=1
             )
 
 
         if self.min_inv == False:
 
             df['ReorderQty'] = df.apply(
                 lambda x: x['RQty'] if x['ReorderStatus'] == 'Order' else 0, axis=1
```

### Comparing `datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/define_periods.py` & `datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/define_periods.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py` & `datupapi-1.97.1/datupapi/inventory/src/ProcessForecast/extract_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py` & `datupapi-1.97.1/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/src/Transformation/inventory_transformation.py` & `datupapi-1.97.1/datupapi/inventory/src/Transformation/inventory_transformation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/inventory/stocks.py` & `datupapi-1.97.1/datupapi/inventory/stocks.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/predict/forecast.py` & `datupapi-1.97.1/datupapi/predict/forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/prepare/cleanse.py` & `datupapi-1.97.1/datupapi/prepare/cleanse.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/prepare/format.py` & `datupapi-1.97.1/datupapi/prepare/format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/prepare/format_dask.py` & `datupapi-1.97.1/datupapi/prepare/format_dask.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/training/attup.py` & `datupapi-1.97.1/datupapi/training/attup.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/training/deepar.py` & `datupapi-1.97.1/datupapi/training/deepar.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/training/tft.py` & `datupapi-1.97.1/datupapi/training/tft.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/transform/backtesting.py` & `datupapi-1.97.1/datupapi/transform/backtesting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/transform/forecasting.py` & `datupapi-1.97.1/datupapi/transform/forecasting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/transform/ranking.py` & `datupapi-1.97.1/datupapi/transform/ranking.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi/utils/utils.py` & `datupapi-1.97.1/datupapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi.egg-info/PKG-INFO` & `datupapi-1.97.1/datupapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.97.0
+Version: 1.97.1
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.97.0/datupapi.egg-info/SOURCES.txt` & `datupapi-1.97.1/datupapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/datupapi.egg-info/requires.txt` & `datupapi-1.97.1/datupapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.97.0/setup.py` & `datupapi-1.97.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='datupapi',
-      version='1.97.0',
+      version='1.97.1',
       description='Utility library to support Datup AI MLOps processes',
       long_description_content_type="text/markdown",
       long_description="foo bar baz",
       author='Datup AI',
       author_email='ramiro@datup.ai',
       packages=[
           'datupapi',
```

