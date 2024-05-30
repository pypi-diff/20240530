# Comparing `tmp/torch_timeseries-0.0.3a1.tar.gz` & `tmp/torch_timeseries-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_timeseries-0.0.3a1.tar", last modified: Thu May 30 05:09:50 2024, max compression
+gzip compressed data, was "torch_timeseries-0.0.3a2.tar", last modified: Thu May 30 05:27:08 2024, max compression
```

## Comparing `torch_timeseries-0.0.3a1.tar` & `torch_timeseries-0.0.3a2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.487733 torch_timeseries-0.0.3a1/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch_timeseries-0.0.3a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19639 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5720 2024-05-29 13:12:27.000000 torch_timeseries-0.0.3a1/README.md
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-25 06:55:33.000000 torch_timeseries-0.0.3a1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 05:09:50.487733 torch_timeseries-0.0.3a1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1162 2024-05-30 05:08:36.000000 torch_timeseries-0.0.3a1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.475733 torch_timeseries-0.0.3a1/torch_timeseries/
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 18:31:12.000000 torch_timeseries-0.0.3a1/torch_timeseries/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.479733 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/
--rw-r--r--   0 root         (0) root         (0)      714 2024-05-29 04:27:55.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5635 2024-05-29 04:25:33.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/anomaly.py
--rw-r--r--   0 root         (0) root         (0)     7261 2024-05-29 04:25:39.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/maskts.py
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-29 04:26:02.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/sliding_window.py
--rw-r--r--   0 root         (0) root         (0)     5954 2024-05-29 04:25:45.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/sliding_window_ts.py
--rw-r--r--   0 root         (0) root         (0)     6950 2024-05-29 04:25:51.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/uea.py
--rw-r--r--   0 root         (0) root         (0)     6550 2024-05-29 04:28:04.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataloader/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/torch_timeseries/dataset/
--rw-r--r--   0 root         (0) root         (0)     1742 2024-05-27 05:33:15.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTh1.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-05-27 05:33:19.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTh2.py
--rw-r--r--   0 root         (0) root         (0)     1802 2024-05-27 05:33:29.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTm1.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-05-27 05:33:34.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTm2.py
--rw-r--r--   0 root         (0) root         (0)     1899 2024-05-27 03:23:05.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/Electricity.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-05-27 05:33:38.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ExchangeRate.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-05-27 06:00:15.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/ILI.py
--rw-r--r--   0 root         (0) root         (0)     2710 2024-05-27 07:36:21.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/M4.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/MSL.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/PSM.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/SMAP.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/SMD.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/SWaT.py
--rw-r--r--   0 root         (0) root         (0)     3445 2024-05-29 12:51:11.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/SolarEnergy.py
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-27 05:33:55.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/Traffic.py
--rw-r--r--   0 root         (0) root         (0)     4741 2024-05-29 03:53:50.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/UEA.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-05-27 05:48:34.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/Weather.py
--rw-r--r--   0 root         (0) root         (0)     1005 2024-05-28 14:34:45.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3025 2024-05-28 14:07:55.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-27 05:40:35.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-27 05:42:01.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/dummy.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-27 05:41:33.000000 torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/dummy_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/torch_timeseries/model/
--rw-r--r--   0 root         (0) root         (0)     3685 2024-05-28 16:33:34.000000 torch_timeseries-0.0.3a1/torch_timeseries/model/DLinear.py
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 09:25:39.000000 torch_timeseries-0.0.3a1/torch_timeseries/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/torch_timeseries/scaler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-29 04:27:08.000000 torch_timeseries-0.0.3a1/torch_timeseries/scaler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1696 2024-05-29 04:22:59.000000 torch_timeseries-0.0.3a1/torch_timeseries/scaler/base.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-29 04:24:45.000000 torch_timeseries-0.0.3a1/torch_timeseries/scaler/maxabs.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 04:24:36.000000 torch_timeseries-0.0.3a1/torch_timeseries/scaler/standard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:09:50.483733 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19639 2024-05-30 05:09:50.000000 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1556 2024-05-30 05:09:50.000000 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 05:09:50.000000 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-30 05:09:50.000000 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 05:09:50.000000 torch_timeseries-0.0.3a1/torch_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.183263 torch_timeseries-0.0.3a2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 14:44:45.000000 torch_timeseries-0.0.3a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19396 2024-05-30 05:27:08.183263 torch_timeseries-0.0.3a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5720 2024-05-29 13:12:27.000000 torch_timeseries-0.0.3a2/README.md
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-25 06:55:33.000000 torch_timeseries-0.0.3a2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 05:27:08.183263 torch_timeseries-0.0.3a2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1162 2024-05-30 05:26:05.000000 torch_timeseries-0.0.3a2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.175263 torch_timeseries-0.0.3a2/torch_timeseries/
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-26 18:31:12.000000 torch_timeseries-0.0.3a2/torch_timeseries/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.175263 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/
+-rw-r--r--   0 root         (0) root         (0)      714 2024-05-29 04:27:55.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5635 2024-05-29 04:25:33.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/anomaly.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2024-05-29 04:25:39.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/maskts.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-29 04:26:02.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/sliding_window.py
+-rw-r--r--   0 root         (0) root         (0)     5954 2024-05-29 04:25:45.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/sliding_window_ts.py
+-rw-r--r--   0 root         (0) root         (0)     6950 2024-05-29 04:25:51.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/uea.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-05-29 04:28:04.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataloader/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.179263 torch_timeseries-0.0.3a2/torch_timeseries/dataset/
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-05-27 05:33:15.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTh1.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-05-27 05:33:19.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTh2.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-05-27 05:33:29.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTm1.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-05-27 05:33:34.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTm2.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2024-05-27 03:23:05.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/Electricity.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-05-27 05:33:38.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ExchangeRate.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-27 06:00:15.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/ILI.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2024-05-27 07:36:21.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/M4.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/MSL.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/PSM.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/SMAP.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/SMD.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-05-29 11:08:47.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/SWaT.py
+-rw-r--r--   0 root         (0) root         (0)     3445 2024-05-29 12:51:11.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/SolarEnergy.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-27 05:33:55.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/Traffic.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2024-05-29 03:53:50.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/UEA.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-05-27 05:48:34.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/Weather.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-05-28 14:34:45.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2024-05-28 14:07:55.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.179263 torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-27 05:40:35.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-27 05:42:01.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/dummy.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-27 05:41:33.000000 torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/dummy_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.179263 torch_timeseries-0.0.3a2/torch_timeseries/model/
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-28 16:33:34.000000 torch_timeseries-0.0.3a2/torch_timeseries/model/DLinear.py
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 09:25:39.000000 torch_timeseries-0.0.3a2/torch_timeseries/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.183263 torch_timeseries-0.0.3a2/torch_timeseries/scaler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-29 04:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries/scaler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-29 04:22:59.000000 torch_timeseries-0.0.3a2/torch_timeseries/scaler/base.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-29 04:24:45.000000 torch_timeseries-0.0.3a2/torch_timeseries/scaler/maxabs.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 04:24:36.000000 torch_timeseries-0.0.3a2/torch_timeseries/scaler/standard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:27:08.175263 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19396 2024-05-30 05:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1556 2024-05-30 05:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 05:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-30 05:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-30 05:27:08.000000 torch_timeseries-0.0.3a2/torch_timeseries.egg-info/top_level.txt
```

### Comparing `torch_timeseries-0.0.3a1/LICENSE` & `torch_timeseries-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/PKG-INFO` & `torch_timeseries-0.0.3a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: torch_timeseries
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3a1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3a2.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,28 +209,20 @@
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
```

### Comparing `torch_timeseries-0.0.3a1/README.md` & `torch_timeseries-0.0.3a2/README.md`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/pyproject.toml` & `torch_timeseries-0.0.3a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/setup.py` & `torch_timeseries-0.0.3a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '0.0.3a1'
+__version__ = '0.0.3a2'
 URL = 'https://github.com/wayne155/pytorch_timeseries'
 
 install_requires = [
     'tqdm',
     'torch',
     'numpy' ,
     'pandas',
```

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/__init__.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/anomaly.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/anomaly.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/maskts.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/maskts.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/sliding_window.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/sliding_window.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/sliding_window_ts.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/sliding_window_ts.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/uea.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/uea.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataloader/wrapper.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataloader/wrapper.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTh1.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTh1.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTh2.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTh2.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTm1.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTm1.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ETTm2.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ETTm2.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/Electricity.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/Electricity.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ExchangeRate.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ExchangeRate.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/ILI.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/ILI.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/M4.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/M4.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/MSL.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/MSL.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/PSM.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/PSM.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/SMAP.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/SMAP.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/SMD.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/SMD.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/SWaT.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/SWaT.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/SolarEnergy.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/SolarEnergy.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/Traffic.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/Traffic.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/UEA.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/UEA.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/Weather.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/Weather.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/__init__.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/dataset.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/dummy.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/dataset/dummies/dummy_graph.py` & `torch_timeseries-0.0.3a2/torch_timeseries/dataset/dummies/dummy_graph.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/model/DLinear.py` & `torch_timeseries-0.0.3a2/torch_timeseries/model/DLinear.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/scaler/base.py` & `torch_timeseries-0.0.3a2/torch_timeseries/scaler/base.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/scaler/maxabs.py` & `torch_timeseries-0.0.3a2/torch_timeseries/scaler/maxabs.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries/scaler/standard.py` & `torch_timeseries-0.0.3a2/torch_timeseries/scaler/standard.py`

 * *Files identical despite different names*

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries.egg-info/PKG-INFO` & `torch_timeseries-0.0.3a2/torch_timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: torch_timeseries
-Version: 0.0.3a1
+Name: torch-timeseries
+Version: 0.0.3a2
 Summary: Timeseries Learning Library for PyTorch.
 Home-page: https://github.com/wayne155/pytorch_timeseries
-Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3a1.tar.gz
+Download-URL: https://github.com/wayne155/pytorch_timeseries/archive/0.0.3a2.tar.gz
 Author: Weiwei Ye
 Author-email: Wayne Yip <wwye155@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -209,28 +209,20 @@
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
```

### Comparing `torch_timeseries-0.0.3a1/torch_timeseries.egg-info/SOURCES.txt` & `torch_timeseries-0.0.3a2/torch_timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

