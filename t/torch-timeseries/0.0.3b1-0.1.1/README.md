# Comparing `tmp/torch_timeseries-0.0.3b1.tar.gz` & `tmp/torch-timeseries-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_timeseries-0.0.3b1.tar", last modified: Thu May 30 05:44:22 2024, max compression
+gzip compressed data, was "torch-timeseries-0.1.1.tar", last modified: Thu May 30 18:04:28 2024, max compression
```

## Comparing `torch_timeseries-0.0.3b1.tar` & `torch-timeseries-0.1.1.tar`

### file list

```diff
@@ -1,62 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch_timeseries-0.0.3b1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19739 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5720 2024-05-29 13:12:27.000000 torch_timeseries-0.0.3b1/README.md
--rw-r--r--   0 root         (0) root         (0)      811 2024-05-30 05:38:50.000000 torch_timeseries-0.0.3b1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1162 2024-05-30 05:44:18.000000 torch_timeseries-0.0.3b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.877534 torch_timeseries-0.0.3b1/torch_timeseries/
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 18:31:12.000000 torch_timeseries-0.0.3b1/torch_timeseries/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.877534 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/
--rw-r--r--   0 root         (0) root         (0)      714 2024-05-29 04:27:55.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5635 2024-05-29 04:25:33.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/anomaly.py
--rw-r--r--   0 root         (0) root         (0)     7261 2024-05-29 04:25:39.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/maskts.py
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-29 04:26:02.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/sliding_window.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-05-29 04:25:45.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/sliding_window_ts.py
--rw-r--r--   0 root         (0) root         (0)     6950 2024-05-29 04:25:51.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/uea.py
--rw-r--r--   0 root         (0) root         (0)     6550 2024-05-29 04:28:04.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataloader/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.881534 torch_timeseries-0.0.3b1/torch_timeseries/dataset/
--rw-r--r--   0 root         (0) root         (0)     1742 2024-05-27 05:33:15.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTh1.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-05-27 05:33:19.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTh2.py
--rw-r--r--   0 root         (0) root         (0)     1802 2024-05-27 05:33:29.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTm1.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-05-27 05:33:34.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTm2.py
--rw-r--r--   0 root         (0) root         (0)     1899 2024-05-27 03:23:05.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/Electricity.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-05-27 05:33:38.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ExchangeRate.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-05-27 06:00:15.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/ILI.py
--rw-r--r--   0 root         (0) root         (0)     2710 2024-05-27 07:36:21.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/M4.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/MSL.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/PSM.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/SMAP.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/SMD.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/SWaT.py
--rw-r--r--   0 root         (0) root         (0)     3445 2024-05-29 12:51:11.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/SolarEnergy.py
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-27 05:33:55.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/Traffic.py
--rw-r--r--   0 root         (0) root         (0)     4741 2024-05-29 03:53:50.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/UEA.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-05-27 05:48:34.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/Weather.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-05-28 14:34:45.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3025 2024-05-28 14:07:55.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.881534 torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-27 05:40:35.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-27 05:42:01.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/dummy.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-27 05:41:33.000000 torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/dummy_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/torch_timeseries/model/
--rw-r--r--   0 root         (0) root         (0)     3685 2024-05-28 16:33:34.000000 torch_timeseries-0.0.3b1/torch_timeseries/model/DLinear.py
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 09:25:39.000000 torch_timeseries-0.0.3b1/torch_timeseries/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/torch_timeseries/nn/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 05:43:04.000000 torch_timeseries-0.0.3b1/torch_timeseries/nn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-05-24 09:15:39.000000 torch_timeseries-0.0.3b1/torch_timeseries/nn/decomp.py
--rw-r--r--   0 root         (0) root         (0)      739 2024-05-24 09:15:09.000000 torch_timeseries-0.0.3b1/torch_timeseries/nn/kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/torch_timeseries/scaler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-29 04:27:08.000000 torch_timeseries-0.0.3b1/torch_timeseries/scaler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1696 2024-05-29 04:22:59.000000 torch_timeseries-0.0.3b1/torch_timeseries/scaler/base.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-29 04:24:45.000000 torch_timeseries-0.0.3b1/torch_timeseries/scaler/maxabs.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 04:24:36.000000 torch_timeseries-0.0.3b1/torch_timeseries/scaler/standard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/torch_timeseries/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 05:42:56.000000 torch_timeseries-0.0.3b1/torch_timeseries/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5686 2024-05-24 08:39:12.000000 torch_timeseries-0.0.3b1/torch_timeseries/utils/timefeatures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:44:22.885534 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19739 2024-05-30 05:44:22.000000 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1723 2024-05-30 05:44:22.000000 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 05:44:22.000000 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-05-30 05:44:22.000000 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 05:44:22.000000 torch_timeseries-0.0.3b1/torch_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.260390 torch-timeseries-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch-timeseries-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    20902 2024-05-30 18:04:28.260390 torch-timeseries-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7230 2024-05-30 17:59:15.000000 torch-timeseries-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      927 2024-05-30 17:08:45.000000 torch-timeseries-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 18:04:28.260390 torch-timeseries-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-05-30 18:03:45.000000 torch-timeseries-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.240390 torch-timeseries-0.1.1/torch_timeseries/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-05-30 16:34:37.000000 torch-timeseries-0.1.1/torch_timeseries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.240390 torch-timeseries-0.1.1/torch_timeseries/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 16:34:22.000000 torch-timeseries-0.1.1/torch_timeseries/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-05-30 16:29:20.000000 torch-timeseries-0.1.1/torch_timeseries/cli/exp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.240390 torch-timeseries-0.1.1/torch_timeseries/core/
+-rw-r--r--   0 root         (0) root         (0)      209 2024-05-30 09:02:37.000000 torch-timeseries-0.1.1/torch_timeseries/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.244390 torch-timeseries-0.1.1/torch_timeseries/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-30 09:02:31.000000 torch-timeseries-0.1.1/torch_timeseries/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-30 07:07:18.000000 torch-timeseries-0.1.1/torch_timeseries/core/dataset/anomaly.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-30 10:37:49.000000 torch-timeseries-0.1.1/torch_timeseries/core/dataset/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.244390 torch-timeseries-0.1.1/torch_timeseries/core/experiments/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 16:49:31.000000 torch-timeseries-0.1.1/torch_timeseries/core/experiments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      843 2024-05-30 10:34:44.000000 torch-timeseries-0.1.1/torch_timeseries/core/experiments/settings.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-30 07:15:52.000000 torch-timeseries-0.1.1/torch_timeseries/core/scaler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.244390 torch-timeseries-0.1.1/torch_timeseries/dataloader/
+-rw-r--r--   0 root         (0) root         (0)      714 2024-05-29 04:27:55.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5792 2024-05-30 16:59:38.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/anomaly.py
+-rw-r--r--   0 root         (0) root         (0)     7277 2024-05-30 09:54:47.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/maskts.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-05-30 09:02:21.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/sliding_window.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2024-05-30 09:11:39.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/sliding_window_ts.py
+-rw-r--r--   0 root         (0) root         (0)     6963 2024-05-30 10:38:14.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/uea.py
+-rw-r--r--   0 root         (0) root         (0)     6562 2024-05-30 09:02:49.000000 torch-timeseries-0.1.1/torch_timeseries/dataloader/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.252390 torch-timeseries-0.1.1/torch_timeseries/dataset/
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-05-30 08:09:04.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ETTh1.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-05-30 09:02:09.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ETTh2.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-05-30 08:10:11.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ETTm1.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-30 08:09:15.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ETTm2.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-05-30 08:08:48.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/Electricity.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-05-30 08:07:46.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ExchangeRate.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-05-30 08:07:48.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/ILI.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2024-05-30 08:07:50.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/M4.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-05-30 08:09:45.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/MSL.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-30 08:09:38.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/PSM.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-05-30 08:09:49.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/SMAP.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-30 08:07:59.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/SMD.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-30 08:08:36.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/SWaT.py
+-rw-r--r--   0 root         (0) root         (0)     3459 2024-05-30 08:08:33.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/SolarEnergy.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-30 08:08:38.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/Traffic.py
+-rw-r--r--   0 root         (0) root         (0)     4755 2024-05-30 10:33:24.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/UEA.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-30 08:08:43.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/Weather.py
+-rw-r--r--   0 root         (0) root         (0)      932 2024-05-30 08:07:14.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.252390 torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-27 05:40:35.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-30 09:01:59.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/dummy.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-30 08:59:57.000000 torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/dummy_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.252390 torch-timeseries-0.1.1/torch_timeseries/experiments/
+-rw-r--r--   0 root         (0) root         (0)     4080 2024-05-30 16:12:26.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/DLinear.py
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-30 16:13:02.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18382 2024-05-30 16:47:58.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/anomaly_detection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 16:23:32.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/base.py
+-rw-r--r--   0 root         (0) root         (0)    16202 2024-05-30 16:47:18.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/forecast.py
+-rw-r--r--   0 root         (0) root         (0)    16288 2024-05-30 16:47:30.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/imputation.py
+-rw-r--r--   0 root         (0) root         (0)    15145 2024-05-30 16:47:45.000000 torch-timeseries-0.1.1/torch_timeseries/experiments/uea_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.256390 torch-timeseries-0.1.1/torch_timeseries/model/
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-28 16:33:34.000000 torch-timeseries-0.1.1/torch_timeseries/model/DLinear.py
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 09:25:39.000000 torch-timeseries-0.1.1/torch_timeseries/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.256390 torch-timeseries-0.1.1/torch_timeseries/nn/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-30 05:43:04.000000 torch-timeseries-0.1.1/torch_timeseries/nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-05-24 09:15:39.000000 torch-timeseries-0.1.1/torch_timeseries/nn/decomp.py
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-24 09:15:09.000000 torch-timeseries-0.1.1/torch_timeseries/nn/kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.256390 torch-timeseries-0.1.1/torch_timeseries/scaler/
+-rw-r--r--   0 root         (0) root         (0)      179 2024-05-30 09:09:12.000000 torch-timeseries-0.1.1/torch_timeseries/scaler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-30 08:10:18.000000 torch-timeseries-0.1.1/torch_timeseries/scaler/maxabs.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2024-05-30 09:09:42.000000 torch-timeseries-0.1.1/torch_timeseries/scaler/standard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.260390 torch-timeseries-0.1.1/torch_timeseries/utils/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-30 10:12:45.000000 torch-timeseries-0.1.1/torch_timeseries/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-30 10:12:57.000000 torch-timeseries-0.1.1/torch_timeseries/utils/acc.py
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-30 07:33:55.000000 torch-timeseries-0.1.1/torch_timeseries/utils/dataclass_ext.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2024-05-30 08:02:47.000000 torch-timeseries-0.1.1/torch_timeseries/utils/early_stop.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-30 08:14:26.000000 torch-timeseries-0.1.1/torch_timeseries/utils/model_stats.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-30 10:35:23.000000 torch-timeseries-0.1.1/torch_timeseries/utils/parse_type.py
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-30 07:26:31.000000 torch-timeseries-0.1.1/torch_timeseries/utils/reproduce.py
+-rw-r--r--   0 root         (0) root         (0)     5686 2024-05-24 08:39:12.000000 torch-timeseries-0.1.1/torch_timeseries/utils/timefeatures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:04:28.240390 torch-timeseries-0.1.1/torch_timeseries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20902 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 18:04:28.000000 torch-timeseries-0.1.1/torch_timeseries.egg-info/top_level.txt
```

### Comparing `torch_timeseries-0.0.3b1/LICENSE` & `torch-timeseries-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/PKG-INFO` & `torch-timeseries-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: torch_timeseries
-Version: 0.0.3b1
+Name: torch-timeseries
+Version: 0.1.1
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3b1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.1.1.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,32 +209,20 @@
            limitations under the License.
         
 Project-URL: Documentation, https://pytorch-timeseries.readthedocs.io
 Project-URL: BugTracker, https://github.com/wayne155/pytorch_timeseries/issues
 Keywords: deep Learning,time series,pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: torchvision
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: sktime
-Requires-Dist: pandas>=0.29.0
-Requires-Dist: scikit-learn
-Requires-Dist: tqdm
 Provides-Extra: full
 Provides-Extra: benchmark
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: g
-Requires-Dist: pyg; extra == "g"
+License-File: LICENSE
 
 [pypi-image]: https://badge.fury.io/py/torch-timeseries.svg
 [pypi-url]: https://pypi.python.org/pypi/torch-timeseries
 [docs-image]: https://readthedocs.org/projects/pytorch-timeseries/badge/?version=latest
 [docs-url]: https://pytorch-timeseries.readthedocs.io/en/latest/?badge=latest
 
 
@@ -244,142 +232,138 @@
 </p>
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
 
 
 
-
-
-
 # pytorch_timeseries
 An all in one deep learning library that boost your timeseries research.
 [Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
 
+
+
 Compared to previous libraries, pytorch_timeseries is 
 - dataset automatically downloaded
 - easy to use and extend 
 - clear documentation 
 - highly customizable 
+- install and run! 
 - ..........
 
 
 
-## installation
+## 1. installation
 
 
 
 ```
 pip install torch-timeseries
 ```
 
 > ⚠️⚠️⚠️ **Warning: We only support python version >= 3.8+**
 
-### addtional install
-For running Graph Nerual Network based models, pytorch_geometric is also needed.
 
-```python
-pip install torch_geometric
+## 2. Running Implemented Experiments
 
-# Optional dependencies
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
+### Forecast
+```python
+# running DLinear Forecast on dataset ETTh1 with seed = 3 
+pytexp --model DLinear --task Forecast --dataset_type ETTh1 run 3
+# running DLinear Forecast on dataset ETTh1 with seeds=[1,2,3]
+pytexp --model DLinear --task Forecast --dataset_type ETTh1 runs '[1,2,3]'
 ```
 
 
-# Quick Start
-
-## 1 Forecasting
-
-### 1.1 download dataset
-The dataset will be downloaded **automatically!!!!**
+### Imputation
 ```python
-from torch_timeseries.dataset import ETTh1
-from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
-from torch_timeseries.model import DLinear
-from torch.nn import MSELoss, L1Loss
-from torch.optim import Adam
-dataset = ETTh1('./data')
+# running DLinear Imputation on dataset ETTh1 with seed = 3 
+pytexp --model DLinear --task Imputation --dataset_type ETTh1 run 3
+# running DLinear Imputation on dataset ETTh1 with seed = [1,2,3] 
+pytexp --model DLinear --task Imputation --dataset_type ETTh1 run '[1,2,3]'
 ```
-
-### 1.2 setup scaler/dataloader
-
-Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
-
-
+### UEAClassification
 ```python
-scaler = StandardScaler()
-dataloader = SlidingWindowTS(dataset, 
-                        window=96,
-                        horizon=1,
-                        steps=336,
-                        batch_size=32, 
-                        train_ratio=0.7, 
-                        val_ratio=0.2, 
-                        scaler=scaler,
-                        )
-
+# running DLinear UEAClassification on dataset EthanolConcentration with seed = 3 
+pytexp --model DLinear --task UEAClassification --dataset_type EthanolConcentration run 3
+# running DLinear UEAClassification on dataset EthanolConcentration with seed = [1,2,3] 
+pytexp --model DLinear --task UEAClassification --dataset_type EthanolConcentration run '[1,2,3]'
 ```
-After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
-
-### 1.3 training
-
-
 
+### AnomalyDetection
 ```python
-model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
-optimizer = Adam(model.parameters())
-loss_function = MSELoss()
-
-# train
-model.train()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
-    optimizer.zero_grad()
-    
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    
-    loss = loss_function(scaled_pred_y, scaled_y)
-    loss.backward()
-    optimizer.step()
-    print(loss)
+# running DLinear AnomalyDetection on dataset MSL with seed = [1,2,3] 
+pytexp --model DLinear --task AnomalyDetection --dataset_type MSL run 3
+# running DLinear AnomalyDetection on dataset MSL with seed = [1,2,3] 
+pytexp --model DLinear --task AnomalyDetection --dataset_type MSL run 3
 ```
 
-### 1.4 val/test
 
-```python
-# val
-model.eval()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
-    ....your validation code here...
-
-# test
-model.eval()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
-    ....your test code here...
-```
+# Development Milestones
+## Implemented Datasets
+Full list of datasets can be found at [Documentation](https://pytorch-timeseries.readthedocs.io/en/latest/modules/dataset.html).
+| Datasets | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [ETTh1](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTh2](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTm1](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTm2](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [......And More](https://pytorch-timeseries.readthedocs.io/en/latest/modules/dataset.html)   | ✅ |✅ | ✅ | ✅ |
+
+## Implemented Tasks
+
+- [x] Forecast
+- [x] Classfication (for UEA datasets)
+- [x] Anomaly Detection 
+- [x] Imputation
+- [ ] You can fill this check box! (contribute to develop your own task!)
+
+## Implemented Models
+
+| Models | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [DLinear (2022)](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |✅ |✅ |
+
+<!-- ## Implemented Datasets
+Currently we have implemented all popular datasets, including
+
+| Datasets | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [ETTh1](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTh2](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTm1](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTm2](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
 
+[Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
+  -->
 
+#  Customizing Your Own Pipeline
 
+we provide examples of :
+- [forecast](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/forecast.py)
+- [imputation](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/mask.py)
+- [anomaly detection](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/anomaly.py)
+- [UEA classfication](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/ueaclass.py)
 
+Detail of customize forecasting pipeline is as follows:
 
-## 2 Imputation
+## 1 Forecasting
 
-### 1. download dataset
+### 1.1 download dataset
 The dataset will be downloaded **automatically!!!!**
 ```python
 from torch_timeseries.dataset import ETTh1
 from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
 from torch_timeseries.model import DLinear
 from torch.nn import MSELoss, L1Loss
 from torch.optim import Adam
 dataset = ETTh1('./data')
 ```
 
-### 2. setup scaler/dataloader
+### 1.2 setup scaler/dataloader
 
 Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
 
 
 ```python
 scaler = StandardScaler()
 dataloader = SlidingWindowTS(dataset, 
@@ -391,15 +375,15 @@
                         val_ratio=0.2, 
                         scaler=scaler,
                         )
 
 ```
 After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
 
-### 3. training
+### 1.3 training
 
 
 
 ```python
 model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 optimizer = Adam(model.parameters())
 loss_function = MSELoss()
@@ -415,45 +399,44 @@
     
     loss = loss_function(scaled_pred_y, scaled_y)
     loss.backward()
     optimizer.step()
     print(loss)
 ```
 
-### 4. val/test
+### 1.4 val/test
 
 ```python
 # val
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    loss = loss_function(scaled_pred_y, scaled_y)
-    
+    ....your validation code here...
 
 # test
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    loss = loss_function(scaled_pred_y, scaled_y)
-    
+    ....your test code here...
 ```
 
 
+# Dev Install 
 
-# dev install 
-
-# install requirements
+## install requirements
 > Note:This library assumes that you've installed Pytorch according to it's official website, the basic dependencies of torch > > related libraries may not be listed in the requirements files:
 https://pytorch.org/get-started/locally/
 
 **The recommended python version is 3.8.1+.**
-Please first install torch according to your environment.
+1. fork this project 
+
+2. clone this project (latest version)
 ```
-pip3 install torch torchvision torchaudio
+git clone https://github.com/wayne155/pytorch_timeseries
 ```
 
+3.  install requirements.
+```
+pip install -r ./requirements.txt
+```
 
+4. change some code and push to the forked repo
 
+5. create a pull request to this repo
```

### Comparing `torch_timeseries-0.0.3b1/pyproject.toml` & `torch-timeseries-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 dynamic = ["version"]
 requires-python = ">= 3.8"
-name = "torch_timeseries"
+name = "torch-timeseries"
 description = "Timeseries Learning Library for PyTorch."
 authors = [{ name = "Wayne Yip", email = "wwye155@gmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["deep Learning", "time series", "pytorch"]
 dependencies = [
     "torch",
     "torchvision",
     "numpy",
     "pandas",
     "sktime",
     "pandas>=0.29.0",
     "scikit-learn",
     "tqdm",
+    "prettytable",
+    "torchmetrics==1.1.1",
+    "fire>=0.5.0"
 ]
 
+[project.scripts]
+pytexp = "torch_timeseries:exp"
+
+
 [project.urls]
 Documentation = "https://pytorch-timeseries.readthedocs.io"
 BugTracker = "https://github.com/wayne155/pytorch_timeseries/issues"
 
 
 [project.optional-dependencies]
 g = ["pyg"]
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/__init__.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/anomaly.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/anomaly.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from ..scaler import Scaler
-from torch_timeseries.dataset import TimeSeriesDataset, AnomalyDataset
+from torch_timeseries.core import TimeSeriesDataset, AnomalyDataset
 from torch.utils.data import Dataset, DataLoader, RandomSampler, Subset
 
 
 class AnomalySliced(TimeSeriesDataset):
     """
     Data loader for anomaly detection in time series datasets.
 
@@ -22,22 +22,22 @@
     """
 
     def __init__(
         self,
         dataset: AnomalyDataset,
         scaler: Scaler,
         train_ratio: float = 0.8,
-        step=1,
-        window: int = 168,
+        spacing=100,
+        window: int = 100,
         scaler_fit=True,
         flag="train",
     ):
         self.dataset = dataset
         self.window = window
-        self.step = step
+        self.spacing = spacing
         self.scaler = scaler
         self.flag = flag
         self.train_ratio = train_ratio
 
         _len = self.dataset.train_data.shape[0]
 
         self.train_len = int(_len * self.train_ratio)
@@ -51,15 +51,15 @@
             self.scaled_val_data = self.scaler.transform(self.val_data)
         elif flag == "test":
             self.test_data = self.dataset.test_data
             self.test_labels = self.dataset.test_labels
             self.scaled_test_data = self.scaler.transform(self.test_data)
 
     def __getitem__(self, index):
-        index = index * self.step
+        index = index * self.spacing
         if self.flag == "train":
             return np.float32(
                 self.scaled_train_data[index : index + self.window]
             ), np.float32(self.train_data[index : index + self.window])
         elif self.flag == "val":
             return (
                 np.float32(self.scaled_val_data[index : index + self.window]),
@@ -72,41 +72,43 @@
                 np.float32(self.test_labels[index : index + self.window]),
             )
         else:
             NotImplementedError("not implemented")
 
     def __len__(self):
         if self.flag == "train":
-            return (self.train_data.shape[0] - self.window) // self.step + 1
+            return (self.train_data.shape[0] - self.window) // self.spacing + 1
         elif self.flag == "val":
-            return (self.val_data.shape[0] - self.window) // self.step + 1
+            return (self.val_data.shape[0] - self.window) // self.spacing + 1
         elif self.flag == "test":
-            return (self.test_data.shape[0] - self.window) // self.step + 1
+            return (self.test_data.shape[0] - self.window) // self.spacing + 1
         else:
             raise NotImplementedError("Not implemented!!!")
 
 
 class AnomalyLoader:
 
     def __init__(
         self,
         dataset: TimeSeriesDataset,
         scaler: Scaler,
-        window: int = 168,
+        window: int = 100,
+        spacing: int = 100,
         shuffle_train=True,
         batch_size: int = 32,
         train_ratio: float = 0.8,
         num_worker: int = 3,
     ) -> None:
 
         self.train_ratio = train_ratio
         self.val_ratio = 1 - self.train_ratio
         self.batch_size = batch_size
         self.num_worker = num_worker
         self.dataset = dataset
+        self.spacing = spacing
 
         self.scaler = scaler
         self.window = window
         self.shuffle_train = shuffle_train
         
         self.train_loader : DataLoader
         self.val_loader : DataLoader
@@ -119,30 +121,33 @@
         self._load_dataloader()
 
     def _load_dataset(self):
         self.train_dataset = AnomalySliced(
             self.dataset,
             self.scaler,
             self.train_ratio,
+            self.spacing,
             self.window,
             scaler_fit=True,
             flag="train",
         )
         self.val_dataset = AnomalySliced(
             self.dataset,
             self.scaler,
             self.train_ratio,
+            self.spacing,
             self.window,
             scaler_fit=False,
             flag="val",
         )
         self.test_dataset = AnomalySliced(
             self.dataset,
             self.scaler,
             self.train_ratio,
+            self.spacing,
             self.window,
             scaler_fit=False,
             flag="test",
         )
 
     def _load_dataloader(self):
         self.train_size = len(self.train_dataset)
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/maskts.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/maskts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Sequence, Tuple, Type
 
 import numpy as np
 import torch
 
 from torch_timeseries.utils.timefeatures import time_features
 from ..scaler import Scaler
-from ..dataset import (
+from torch_timeseries.core import (
     TimeSeriesDataset,
     TimeseriesSubset,
 )
 from torch.utils.data import Dataset, DataLoader, RandomSampler, Subset
 
 from .wrapper import MultiStepTimeFeatureSet
 
@@ -92,15 +92,15 @@
     def __init__(
         self,
         dataset: TimeSeriesDataset,
         scaler: Scaler,
         time_enc=0,
         window: int = 168,
         mask_rate=0.4,
-        scale_in_train=False,
+        scale_in_train=True,
         shuffle_train=True,
         freq=None,
         batch_size: int = 32,
         train_ratio: float = 0.7,
         val_ratio: float = 0.2,
         num_worker: int = 3,
         uniform_eval=True,
@@ -157,15 +157,15 @@
 
         if self.uniform_eval:
             test_subset = TimeseriesSubset(self.dataset, indices[-test_size - self.window:])
         else:
             test_subset = TimeseriesSubset(self.dataset, indices[-test_size:])
 
         if self.scale_in_train:
-            self.scaler.fit(train_subset)
+            self.scaler.fit(train_subset.data)
         else:
             self.scaler.fit(self.dataset.data)
 
         self.train_dataset = MaskTimeFeatureSet(
             train_subset,
             scaler=self.scaler,
             time_enc=self.time_enc,
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/sliding_window.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/sliding_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence, Tuple, Type
 
 import torch
 from ..scaler import Scaler
-from torch_timeseries.dataset import (
+from torch_timeseries.core import (
     TimeSeriesDataset,
     TimeseriesSubset,
 )
 from torch.utils.data import Dataset, DataLoader, RandomSampler, Subset
 
 from .wrapper import MultiStepTimeFeatureSet, MultiStepSet
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/sliding_window_ts.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/sliding_window_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence, Tuple, Type
 
 import torch
 from ..scaler import Scaler
-from ..dataset import (
+from torch_timeseries.core import (
     TimeSeriesDataset,
     TimeseriesSubset,
 )
 from torch.utils.data import Dataset, DataLoader, RandomSampler, Subset
 
 from .wrapper import MultiStepTimeFeatureSet
 
@@ -107,15 +107,15 @@
         if self.uniform_eval:
             test_subset = TimeseriesSubset(self.dataset, indices[-test_size - self.window - self.horizon + 1:])
         else:
             test_subset = TimeseriesSubset(self.dataset, indices[-test_size:])
 
             
         if self.scale_in_train:
-            self.scaler.fit(train_subset)
+            self.scaler.fit(train_subset.data)
         else:
             self.scaler.fit(self.dataset.data)
 
         self.train_dataset = MultiStepTimeFeatureSet(
             train_subset,
             scaler=self.scaler,
             time_enc=self.time_enc,
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/uea.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/uea.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import torch
 
 from torch_timeseries.dataset import UEA
 from torch_timeseries.utils.timefeatures import time_features
 from ..scaler import Scaler
-from ..dataset import (
+from torch_timeseries.core import (
     TimeSeriesDataset,
     TimeseriesSubset,
 )
 from torch.utils.data import Dataset, DataLoader, RandomSampler, Subset
 
 from .wrapper import MultiStepTimeFeatureSet
 
@@ -20,25 +20,26 @@
 
 class UEADataset(Dataset):
     def __init__(self, dataset: UEA, scaler: Scaler, flag: str ='train', window: int = 168, scaler_fit=True):
         self.dataset = dataset
         self.window = window
         self.scaler = scaler
         self.flag = flag
-        if scaler_fit:
-            self.scaler.fit(self.dataset.train_features_data)
         if self.flag == 'test':
             self.scaled_feature_df = self.scaler.transform(self.dataset.test_df)
             self.feature_df = self.dataset.test_df
             self.labels = self.dataset.test_labels
         elif self.flag == 'train':
+            if scaler_fit:
+                self.scaler.fit(self.dataset.train_features_data)
+
             self.scaled_feature_df = self.scaler.transform(self.dataset.train_df)
             self.feature_df = self.dataset.train_df
             self.labels = self.dataset.train_labels
-        
+
         self.indexes = self.feature_df.index.unique()
         
     def __getitem__(self, ind):
         scaled_x = torch.tensor(self.scaled_feature_df.loc[ind].values)
         x = torch.tensor(self.feature_df.loc[ind].values)
         y = torch.tensor(self.labels.loc[ind].values)
         return scaled_x, x, y
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataloader/wrapper.py` & `torch-timeseries-0.1.1/torch_timeseries/dataloader/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, TypeVar, Tuple
 
 import pandas as pd
 from ..scaler import Scaler
 
 from torch_timeseries.utils.timefeatures import time_features
-from ..dataset import TimeSeriesDataset, TimeseriesSubset
+from torch_timeseries.core import TimeSeriesDataset, TimeseriesSubset
 from torch.utils.data import Dataset
 import numpy as np
 import torch
 
 
 class MultiStepTimeFeatureSet(Dataset):
     def __init__(self, dataset: TimeseriesSubset, scaler: Scaler, time_enc=0, window: int = 168, horizon: int = 3, steps: int = 2, freq=None, scaler_fit=True):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTh1.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ETTh1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, Freq, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, Freq, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_url, download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTh2.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ETTh2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, Freq, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset, Freq
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import (
     download_url,
     download_and_extract_archive,
     check_integrity,
 )
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTm1.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ETTm1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, Freq, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset, Freq
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_url, download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ETTm2.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ETTm2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, Freq, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset, Freq
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_url, download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/Electricity.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/Electricity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity, download_url
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ExchangeRate.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ExchangeRate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity, download_url
 import torch
 from typing import Any, Callable, List, Optional
 import os
 import resource
-from.dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 
 
 class ExchangeRate(TimeSeriesDataset):
     """
     The collection of the daily exchange rates of eight foreign countries including Australia, British, Canada, Switzerland, China, Japan, New Zealand, and Singapore ranging from 1990 to 2016.
     
     The raw data is collected from https://github.com/laiguokun/multivariate-time-series-data.
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/ILI.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/ILI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_url, download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/M4.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/M4.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://github.com/Mcompetitions/M4-methods/tree/master/Dataset
 
 
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import (
     download_url,
     download_and_extract_archive,
     check_integrity,
 )
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/MSL.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/MSL.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset, AnomalyDataset
+from ..core.dataset import AnomalyDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class MSL(AnomalyDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/PSM.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/PSM.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset, AnomalyDataset
+from ..core.dataset import AnomalyDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class PSM(AnomalyDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/SMAP.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/SMAP.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset, AnomalyDataset
+from ..core.dataset import AnomalyDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class SMAP(AnomalyDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/SMD.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/SMD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class SMD(TimeSeriesDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/SWaT.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/SWaT.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class SWaT(TimeSeriesDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/SolarEnergy.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/SolarEnergy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import torch
 from typing import Callable, List, Optional
 import os
 import resource
 import numpy as np
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 
 
 class SolarEnergy(TimeSeriesDataset):
     """
     The dataset contains solar power production records for the year 2006, sampled every 5 minutes from 137 PV plants in Alabama State.
     The raw data is available at http://www.nrel.gov/grid/solar-power-data.html.
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/Traffic.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/Traffic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 
 class Traffic(TimeSeriesDataset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/UEA.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/UEA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sktime.datasets import load_from_tsfile_to_dataframe
 
 
 import os
 import resource
-from .dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import (
     download_url,
     download_and_extract_archive,
     check_integrity,
 )
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/Weather.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/Weather.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import resource
-from.dataset import Dataset, TimeSeriesDataset
+from ..core.dataset.dataset import Dataset, TimeSeriesDataset
 from typing import Any, Callable, List, Optional
 import torch
 from torchvision.datasets.utils import download_url, download_and_extract_archive, check_integrity
 import pandas as pd
 import numpy as np
 import torch.utils.data
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/__init__.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .dummies import Dummy, DummyGraph
-from .dataset import TimeSeriesDataset, TimeseriesSubset, AnomalyDataset
 from .Traffic import Traffic
 from .ExchangeRate import ExchangeRate
 from .SolarEnergy import SolarEnergy
 from .Electricity import Electricity
 from .ETTh1 import ETTh1
 from .ETTh2 import ETTh2
 from .ETTm1 import ETTm1
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/dataset.py` & `torch-timeseries-0.1.1/torch_timeseries/core/dataset/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,22 @@
         return len(self.data)
 
 
 # StoreTypes = Union[np.ndarray, Tensor]
 StoreTypes = np.ndarray
 
 
+
+from abc import abstractmethod
+import os
+from typing import Optional
+
+import pandas as pd
+from .dataset import Dataset, StoreTypes
+
 class TimeSeriesDataset(Dataset):
     def __init__(self, root: str='./data'):
         """_summary_
 
         Args:
             root (str): data save location
 
@@ -77,35 +85,27 @@
         raise NotImplementedError
 
     def _process(self) :
         pass
     
     
     @abstractmethod
-    def _load(self) -> StoreTypes:
+    def _load(self):
         """Loads the dataset to the :attr:`self.data` .
 
         Raises:
             NotImplementedError: _description_
 
         Returns:
             T: should return a numpy.array or torch.tensor or pandas.Dataframe
         """
 
         raise NotImplementedError
 
 
-
-class AnomalyDataset(TimeSeriesDataset):
-    train_data : Optional[np.array]
-    test_data : Optional[np.array]
-    test_labels : Optional[np.array]
-        
-        
-
 class TimeSeriesStaticGraphDataset(TimeSeriesDataset):
     adj : np.ndarray 
     def _load_static_graph(self):
         raise NotImplementedError()
 
 
 class TimeseriesSubset(torch.utils.data.Subset):
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/dummy.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/dummy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 import numpy as np
 import pandas as pd
-from torch_timeseries.dataset.dataset import Freq, TimeSeriesDataset, TimeSeriesStaticGraphDataset
+from torch_timeseries.core import Freq, TimeSeriesDataset, TimeSeriesStaticGraphDataset
 
 
 class Dummy(TimeSeriesDataset):
     """
     Dummy dataset for testing purposes.
 
     Attributes:
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/dataset/dummies/dummy_graph.py` & `torch-timeseries-0.1.1/torch_timeseries/dataset/dummies/dummy_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 import numpy as np
 import pandas as pd
-from torch_timeseries.dataset.dataset import Freq, TimeSeriesDataset, TimeSeriesStaticGraphDataset
+from torch_timeseries.core import Freq, TimeSeriesDataset, TimeSeriesStaticGraphDataset
 
 
 class DummyGraph(TimeSeriesStaticGraphDataset):
     """
     Dummy graph dataset for testing purposes.
 
     Attributes:
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/model/DLinear.py` & `torch-timeseries-0.1.1/torch_timeseries/model/DLinear.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/nn/decomp.py` & `torch-timeseries-0.1.1/torch_timeseries/nn/decomp.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/nn/kernels.py` & `torch-timeseries-0.1.1/torch_timeseries/nn/kernels.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/scaler/base.py` & `torch-timeseries-0.1.1/torch_timeseries/core/scaler.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/scaler/maxabs.py` & `torch-timeseries-0.1.1/torch_timeseries/scaler/maxabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import Tensor
 from typing import Generic, TypeVar, Union
-from .base import Scaler, StoreType
+from ..core.scaler import Scaler, StoreType
 import pandas as pd
 import numpy as np
 import torch
 
 class MaxAbsScaler(Scaler[StoreType]):
     """
     shape of data :  (N , n)
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/scaler/standard.py` & `torch-timeseries-0.1.1/torch_timeseries/scaler/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import Tensor
 from typing import Generic, TypeVar, Union
-from .base import Scaler, StoreType
+from ..core.scaler import Scaler, StoreType
 import pandas as pd
 import numpy as np
 import torch
 
 
 class StandardScaler(Scaler):
     """
```

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries/utils/timefeatures.py` & `torch-timeseries-0.1.1/torch_timeseries/utils/timefeatures.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3b1/torch_timeseries.egg-info/PKG-INFO` & `torch-timeseries-0.1.1/torch_timeseries.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: torch_timeseries
-Version: 0.0.3b1
+Name: torch-timeseries
+Version: 0.1.1
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3b1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.1.1.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,32 +209,20 @@
            limitations under the License.
         
 Project-URL: Documentation, https://pytorch-timeseries.readthedocs.io
 Project-URL: BugTracker, https://github.com/wayne155/pytorch_timeseries/issues
 Keywords: deep Learning,time series,pytorch
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: torchvision
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: sktime
-Requires-Dist: pandas>=0.29.0
-Requires-Dist: scikit-learn
-Requires-Dist: tqdm
 Provides-Extra: full
 Provides-Extra: benchmark
 Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: g
-Requires-Dist: pyg; extra == "g"
+License-File: LICENSE
 
 [pypi-image]: https://badge.fury.io/py/torch-timeseries.svg
 [pypi-url]: https://pypi.python.org/pypi/torch-timeseries
 [docs-image]: https://readthedocs.org/projects/pytorch-timeseries/badge/?version=latest
 [docs-url]: https://pytorch-timeseries.readthedocs.io/en/latest/?badge=latest
 
 
@@ -244,142 +232,138 @@
 </p>
 
 [![PyPI Version][pypi-image]][pypi-url]
 [![Docs Status][docs-image]][docs-url]
 
 
 
-
-
-
 # pytorch_timeseries
 An all in one deep learning library that boost your timeseries research.
 [Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
 
+
+
 Compared to previous libraries, pytorch_timeseries is 
 - dataset automatically downloaded
 - easy to use and extend 
 - clear documentation 
 - highly customizable 
+- install and run! 
 - ..........
 
 
 
-## installation
+## 1. installation
 
 
 
 ```
 pip install torch-timeseries
 ```
 
 > ⚠️⚠️⚠️ **Warning: We only support python version >= 3.8+**
 
-### addtional install
-For running Graph Nerual Network based models, pytorch_geometric is also needed.
 
-```python
-pip install torch_geometric
+## 2. Running Implemented Experiments
 
-# Optional dependencies
-pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
+### Forecast
+```python
+# running DLinear Forecast on dataset ETTh1 with seed = 3 
+pytexp --model DLinear --task Forecast --dataset_type ETTh1 run 3
+# running DLinear Forecast on dataset ETTh1 with seeds=[1,2,3]
+pytexp --model DLinear --task Forecast --dataset_type ETTh1 runs '[1,2,3]'
 ```
 
 
-# Quick Start
-
-## 1 Forecasting
-
-### 1.1 download dataset
-The dataset will be downloaded **automatically!!!!**
+### Imputation
 ```python
-from torch_timeseries.dataset import ETTh1
-from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
-from torch_timeseries.model import DLinear
-from torch.nn import MSELoss, L1Loss
-from torch.optim import Adam
-dataset = ETTh1('./data')
+# running DLinear Imputation on dataset ETTh1 with seed = 3 
+pytexp --model DLinear --task Imputation --dataset_type ETTh1 run 3
+# running DLinear Imputation on dataset ETTh1 with seed = [1,2,3] 
+pytexp --model DLinear --task Imputation --dataset_type ETTh1 run '[1,2,3]'
 ```
-
-### 1.2 setup scaler/dataloader
-
-Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
-
-
+### UEAClassification
 ```python
-scaler = StandardScaler()
-dataloader = SlidingWindowTS(dataset, 
-                        window=96,
-                        horizon=1,
-                        steps=336,
-                        batch_size=32, 
-                        train_ratio=0.7, 
-                        val_ratio=0.2, 
-                        scaler=scaler,
-                        )
-
+# running DLinear UEAClassification on dataset EthanolConcentration with seed = 3 
+pytexp --model DLinear --task UEAClassification --dataset_type EthanolConcentration run 3
+# running DLinear UEAClassification on dataset EthanolConcentration with seed = [1,2,3] 
+pytexp --model DLinear --task UEAClassification --dataset_type EthanolConcentration run '[1,2,3]'
 ```
-After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
-
-### 1.3 training
-
-
 
+### AnomalyDetection
 ```python
-model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
-optimizer = Adam(model.parameters())
-loss_function = MSELoss()
-
-# train
-model.train()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.train_loader:
-    optimizer.zero_grad()
-    
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    
-    loss = loss_function(scaled_pred_y, scaled_y)
-    loss.backward()
-    optimizer.step()
-    print(loss)
+# running DLinear AnomalyDetection on dataset MSL with seed = [1,2,3] 
+pytexp --model DLinear --task AnomalyDetection --dataset_type MSL run 3
+# running DLinear AnomalyDetection on dataset MSL with seed = [1,2,3] 
+pytexp --model DLinear --task AnomalyDetection --dataset_type MSL run 3
 ```
 
-### 1.4 val/test
 
-```python
-# val
-model.eval()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
-    ....your validation code here...
-
-# test
-model.eval()
-for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
-    ....your test code here...
-```
+# Development Milestones
+## Implemented Datasets
+Full list of datasets can be found at [Documentation](https://pytorch-timeseries.readthedocs.io/en/latest/modules/dataset.html).
+| Datasets | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [ETTh1](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTh2](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTm1](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [ETTm2](https://ojs.aaai.org/index.php/AAAI/article/view/17325)   | ✅ |✅ |  |  |
+| [......And More](https://pytorch-timeseries.readthedocs.io/en/latest/modules/dataset.html)   | ✅ |✅ | ✅ | ✅ |
+
+## Implemented Tasks
+
+- [x] Forecast
+- [x] Classfication (for UEA datasets)
+- [x] Anomaly Detection 
+- [x] Imputation
+- [ ] You can fill this check box! (contribute to develop your own task!)
+
+## Implemented Models
+
+| Models | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [DLinear (2022)](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |✅ |✅ |
+
+<!-- ## Implemented Datasets
+Currently we have implemented all popular datasets, including
+
+| Datasets | Forecasting | Imputation | Anomaly | Classification|
+| --------- | ------- | ------- | ------- | ------- |
+| [ETTh1](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTh2](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTm1](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
+| [ETTm2](https://ojs.aaai.org/index.php/AAAI/article/view/26317)   | ✅ |✅ |  |  |
 
+[Check the documentation for more detail](https://pytorch-timeseries.readthedocs.io/en/latest/).
+  -->
 
+#  Customizing Your Own Pipeline
 
+we provide examples of :
+- [forecast](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/forecast.py)
+- [imputation](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/mask.py)
+- [anomaly detection](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/anomaly.py)
+- [UEA classfication](https://github.com/wayne155/pytorch_timeseries/blob/main/examples/ueaclass.py)
 
+Detail of customize forecasting pipeline is as follows:
 
-## 2 Imputation
+## 1 Forecasting
 
-### 1. download dataset
+### 1.1 download dataset
 The dataset will be downloaded **automatically!!!!**
 ```python
 from torch_timeseries.dataset import ETTh1
 from torch_timeseries.dataloader import StandardScaler, SlidingWindow, SlidingWindowTS
 from torch_timeseries.model import DLinear
 from torch.nn import MSELoss, L1Loss
 from torch.optim import Adam
 dataset = ETTh1('./data')
 ```
 
-### 2. setup scaler/dataloader
+### 1.2 setup scaler/dataloader
 
 Once you setup a dataloader and pass a scaler into this dataloader, the scaler will be fitted on the training set.
 
 
 ```python
 scaler = StandardScaler()
 dataloader = SlidingWindowTS(dataset, 
@@ -391,15 +375,15 @@
                         val_ratio=0.2, 
                         scaler=scaler,
                         )
 
 ```
 After this, you can access the train/val/test loader by `dataloader.train_loader/val_loader/test_loader` 
 
-### 3. training
+### 1.3 training
 
 
 
 ```python
 model = DLinear(dataloader.window, dataloader.steps, dataset.num_features, individual= True)
 optimizer = Adam(model.parameters())
 loss_function = MSELoss()
@@ -415,45 +399,44 @@
     
     loss = loss_function(scaled_pred_y, scaled_y)
     loss.backward()
     optimizer.step()
     print(loss)
 ```
 
-### 4. val/test
+### 1.4 val/test
 
 ```python
 # val
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.val_loader:
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    loss = loss_function(scaled_pred_y, scaled_y)
-    
+    ....your validation code here...
 
 # test
 model.eval()
 for scaled_x, scaled_y, x, y, x_date_enc, y_date_enc in dataloader.test_loader:
-    scaled_x = scaled_x.float()
-    scaled_y = scaled_y.float()
-    scaled_pred_y = model(scaled_x) 
-    loss = loss_function(scaled_pred_y, scaled_y)
-    
+    ....your test code here...
 ```
 
 
+# Dev Install 
 
-# dev install 
-
-# install requirements
+## install requirements
 > Note:This library assumes that you've installed Pytorch according to it's official website, the basic dependencies of torch > > related libraries may not be listed in the requirements files:
 https://pytorch.org/get-started/locally/
 
 **The recommended python version is 3.8.1+.**
-Please first install torch according to your environment.
+1. fork this project 
+
+2. clone this project (latest version)
 ```
-pip3 install torch torchvision torchaudio
+git clone https://github.com/wayne155/pytorch_timeseries
 ```
 
+3.  install requirements.
+```
+pip install -r ./requirements.txt
+```
 
+4. change some code and push to the forked repo
 
+5. create a pull request to this repo
```

