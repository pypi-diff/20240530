# Comparing `tmp/hftbacktest-1.8.2.tar.gz` & `tmp/hftbacktest-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.8.2.tar", last modified: Sun May 19 13:48:08 2024, max compression
+gzip compressed data, was "hftbacktest-1.8.3.tar", last modified: Thu May 30 15:43:05 2024, max compression
```

## Comparing `hftbacktest-1.8.2.tar` & `hftbacktest-1.8.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8022 2024-04-24 14:24:53.000000 hftbacktest-1.8.2/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.818140 hftbacktest-1.8.2/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-05-19 12:10:25.000000 hftbacktest-1.8.2/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.2/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.819140 hftbacktest-1.8.2/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1766 2024-05-19 12:10:07.000000 hftbacktest-1.8.2/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.820140 hftbacktest-1.8.2/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14082 2024-04-24 10:45:33.000000 hftbacktest-1.8.2/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.2/hftbacktest/data/utils/binancehistmktdata.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.2/hftbacktest/data/utils/difforderbooksnapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-05-19 12:43:38.000000 hftbacktest-1.8.2/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10184 2024-04-24 14:11:01.000000 hftbacktest-1.8.2/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    17614 2024-05-19 12:15:47.000000 hftbacktest-1.8.2/hftbacktest/data/validation.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.2/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.2/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.2/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.2/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.821140 hftbacktest-1.8.2/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.2/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.2/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30419 2024-04-14 14:19:28.000000 hftbacktest-1.8.2/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.2/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.2/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13980 2023-12-10 12:16:12.000000 hftbacktest-1.8.2/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.2/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.2/hftbacktest/stats.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.2/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-19 13:48:08.819140 hftbacktest-1.8.2/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9133 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1022 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.2/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-05-19 13:48:08.000000 hftbacktest-1.8.2/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1250 2024-05-19 13:48:08.822140 hftbacktest-1.8.2/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.2/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.718188 hftbacktest-1.8.3/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9395 2024-05-30 15:43:05.719188 hftbacktest-1.8.3/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8285 2024-05-26 12:09:21.000000 hftbacktest-1.8.3/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.717188 hftbacktest-1.8.3/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12124 2024-05-30 15:40:04.000000 hftbacktest-1.8.3/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    16000 2024-03-19 13:08:02.000000 hftbacktest-1.8.3/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.717188 hftbacktest-1.8.3/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1766 2024-05-19 12:10:07.000000 hftbacktest-1.8.3/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.718188 hftbacktest-1.8.3/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14148 2024-05-30 14:36:21.000000 hftbacktest-1.8.3/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10189 2024-03-22 14:34:52.000000 hftbacktest-1.8.3/hftbacktest/data/utils/binancehistmktdata.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7967 2023-12-10 12:15:55.000000 hftbacktest-1.8.3/hftbacktest/data/utils/difforderbooksnapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2768 2024-05-19 12:43:38.000000 hftbacktest-1.8.3/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10250 2024-05-30 14:36:21.000000 hftbacktest-1.8.3/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    17614 2024-05-19 12:15:47.000000 hftbacktest-1.8.3/hftbacktest/data/validation.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-08-23 14:57:13.000000 hftbacktest-1.8.3/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.718188 hftbacktest-1.8.3/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    12224 2023-12-10 12:16:05.000000 hftbacktest-1.8.3/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4867 2024-02-14 09:48:00.000000 hftbacktest-1.8.3/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4856 2024-03-11 14:20:26.000000 hftbacktest-1.8.3/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.718188 hftbacktest-1.8.3/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     8149 2023-12-04 12:17:36.000000 hftbacktest-1.8.3/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.8.3/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    30419 2024-04-14 14:19:28.000000 hftbacktest-1.8.3/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5850 2023-12-01 13:42:13.000000 hftbacktest-1.8.3/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3332 2024-03-19 12:28:56.000000 hftbacktest-1.8.3/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14154 2024-05-30 14:01:32.000000 hftbacktest-1.8.3/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.8.3/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.8.3/hftbacktest/stats.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.8.3/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2024-05-30 15:43:05.717188 hftbacktest-1.8.3/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     9395 2024-05-30 15:43:05.000000 hftbacktest-1.8.3/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1022 2024-05-30 15:43:05.000000 hftbacktest-1.8.3/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2024-05-30 15:43:05.000000 hftbacktest-1.8.3/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.8.3/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2024-05-30 15:43:05.000000 hftbacktest-1.8.3/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2024-05-30 15:43:05.000000 hftbacktest-1.8.3/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1250 2024-05-30 15:43:05.719188 hftbacktest-1.8.3/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.8.3/setup.py
```

### Comparing `hftbacktest-1.8.2/LICENSE` & `hftbacktest-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/PKG-INFO` & `hftbacktest-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.2
+Version: 1.8.3
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -159,16 +159,18 @@
 
 Tutorials
 =========
 * `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_
 * `Getting Started <https://hftbacktest.readthedocs.io/en/latest/tutorials/Getting%20Started.html>`_
 * `Working with Market Depth and Trades <https://hftbacktest.readthedocs.io/en/latest/tutorials/Working%20with%20Market%20Depth%20and%20Trades.html>`_
 * `Integrating Custom Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Integrating%20Custom%20Data.html>`_
+* `Making Multiple Markets - Introduction <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets%20-%20Introduction.html>`_
 * `High-Frequency Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/High-Frequency%20Grid%20Trading.html>`_
 * `Impact of Order Latency <https://hftbacktest.readthedocs.io/en/latest/tutorials/Impact%20of%20Order%20Latency.html>`_
+* `Order Latency Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Order%20Latency%20Data.html>`_
 * `Guéant–Lehalle–Fernandez-Tapia Market Making Model and Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/GLFT%20Market%20Making%20Model%20and%20Grid%20Trading.html>`_
 * `Making Multiple Markets <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets.html>`_
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
```

### Comparing `hftbacktest-1.8.2/README.rst` & `hftbacktest-1.8.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -133,16 +133,18 @@
 
 Tutorials
 =========
 * `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_
 * `Getting Started <https://hftbacktest.readthedocs.io/en/latest/tutorials/Getting%20Started.html>`_
 * `Working with Market Depth and Trades <https://hftbacktest.readthedocs.io/en/latest/tutorials/Working%20with%20Market%20Depth%20and%20Trades.html>`_
 * `Integrating Custom Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Integrating%20Custom%20Data.html>`_
+* `Making Multiple Markets - Introduction <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets%20-%20Introduction.html>`_
 * `High-Frequency Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/High-Frequency%20Grid%20Trading.html>`_
 * `Impact of Order Latency <https://hftbacktest.readthedocs.io/en/latest/tutorials/Impact%20of%20Order%20Latency.html>`_
+* `Order Latency Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Order%20Latency%20Data.html>`_
 * `Guéant–Lehalle–Fernandez-Tapia Market Making Model and Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/GLFT%20Market%20Making%20Model%20and%20Grid%20Trading.html>`_
 * `Making Multiple Markets <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets.html>`_
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
 
@@ -188,8 +190,8 @@
 
 .. |docs| image:: https://readthedocs.org/projects/hftbacktest/badge/?version=latest
     :target: https://hftbacktest.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |github| image:: https://img.shields.io/github/stars/nkaz001/hftbacktest?style=social
     :target: https://github.com/nkaz001/hftbacktest
-    :alt: Github
+    :alt: Github
```

### Comparing `hftbacktest-1.8.2/hftbacktest/__init__.py` & `hftbacktest-1.8.3/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.8.2'
+__version__ = '1.8.3'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.8.2/hftbacktest/assettype.py` & `hftbacktest-1.8.3/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/backtest.py` & `hftbacktest-1.8.3/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/data/__init__.py` & `hftbacktest-1.8.3/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.8.3/hftbacktest/data/utils/binancefutures.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,16 @@
     if not structured_array:
         # Validate again.
         num_corr = validate_data(data)
         if num_corr < 0:
             raise ValueError
 
     if structured_array:
-        data = convert_to_struct_arr(data)
+        # EXCH_EVENT and LOCAL_EVENT are already applied.
+        data = convert_to_struct_arr(data, False)
 
     if output_filename is not None:
         print('Saving to %s' % output_filename)
         if compress:
             np.savez_compressed(output_filename, data=data)
         else:
             np.savez(output_filename, data=data)
```

### Comparing `hftbacktest-1.8.2/hftbacktest/data/utils/binancehistmktdata.py` & `hftbacktest-1.8.3/hftbacktest/data/utils/binancehistmktdata.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/data/utils/difforderbooksnapshot.py` & `hftbacktest-1.8.3/hftbacktest/data/utils/difforderbooksnapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.8.3/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.8.3/hftbacktest/data/utils/tardis.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,16 @@
     if not structured_array:
         # Validate again.
         num_corr = validate_data(data)
         if num_corr < 0:
             raise ValueError
 
     if structured_array:
-        data = convert_to_struct_arr(data)
+        # EXCH_EVENT and LOCAL_EVENT are already applied.
+        data = convert_to_struct_arr(data, False)
 
     if output_filename is not None:
         print('Saving to %s' % output_filename)
         if compress:
             np.savez_compressed(output_filename, data=data)
         else:
             np.savez(output_filename, data=data)
```

### Comparing `hftbacktest-1.8.2/hftbacktest/data/validation.py` & `hftbacktest-1.8.3/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/marketdepth.py` & `hftbacktest-1.8.3/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/models/latencies.py` & `hftbacktest-1.8.3/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/models/queue.py` & `hftbacktest-1.8.3/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/order.py` & `hftbacktest-1.8.3/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/proc/local.py` & `hftbacktest-1.8.3/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.8.3/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.8.3/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/proc/proc.py` & `hftbacktest-1.8.3/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/reader.py` & `hftbacktest-1.8.3/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/stat.py` & `hftbacktest-1.8.3/hftbacktest/stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,16 @@
             print('Max. draw down: %.2f %%' % (mdd / capital * 100))
         else:
             print('Annualised return: %.2f' % ar)
             print('Max. draw down: %.2f' % mdd)
         print('The number of trades per day: %d' % dtn)
         print('Avg. daily trading volume: %d' % dtq)
         print('Avg. daily trading amount: %d' % dta)
+        print('Avg. daily turnover (trading amount/capital): %.2f %%' % dta / capital * 100)
+        print('Return per trade (bp): %.2f' % ar / (dta * trading_days) * 10000)
 
         position = np.asarray(self.position) * np.asarray(self.mid)
         if capital is not None:
             print('Max leverage: %.2f' % (np.max(np.abs(position)) / capital))
             print('Median leverage: %.2f' % (np.median(np.abs(position)) / capital))
 
         fig, axs = plt.subplots(2, 1, sharex=True)
```

### Comparing `hftbacktest-1.8.2/hftbacktest/state.py` & `hftbacktest-1.8.3/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/stats.py` & `hftbacktest-1.8.3/hftbacktest/stats.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest/typing.py` & `hftbacktest-1.8.3/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.8.3/hftbacktest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.8.2
+Version: 1.8.3
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -159,16 +159,18 @@
 
 Tutorials
 =========
 * `Data Preparation <https://hftbacktest.readthedocs.io/en/latest/tutorials/Data%20Preparation.html>`_
 * `Getting Started <https://hftbacktest.readthedocs.io/en/latest/tutorials/Getting%20Started.html>`_
 * `Working with Market Depth and Trades <https://hftbacktest.readthedocs.io/en/latest/tutorials/Working%20with%20Market%20Depth%20and%20Trades.html>`_
 * `Integrating Custom Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Integrating%20Custom%20Data.html>`_
+* `Making Multiple Markets - Introduction <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets%20-%20Introduction.html>`_
 * `High-Frequency Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/High-Frequency%20Grid%20Trading.html>`_
 * `Impact of Order Latency <https://hftbacktest.readthedocs.io/en/latest/tutorials/Impact%20of%20Order%20Latency.html>`_
+* `Order Latency Data <https://hftbacktest.readthedocs.io/en/latest/tutorials/Order%20Latency%20Data.html>`_
 * `Guéant–Lehalle–Fernandez-Tapia Market Making Model and Grid Trading <https://hftbacktest.readthedocs.io/en/latest/tutorials/GLFT%20Market%20Making%20Model%20and%20Grid%20Trading.html>`_
 * `Making Multiple Markets <https://hftbacktest.readthedocs.io/en/latest/tutorials/Making%20Multiple%20Markets.html>`_
 * `Risk Mitigation through Price Protection in Extreme Market Conditions <https://hftbacktest.readthedocs.io/en/latest/tutorials/Risk%20Mitigation%20through%20Price%20Protection%20in%20Extreme%20Market%20Conditions.html>`_
 
 Examples
 ========
```

### Comparing `hftbacktest-1.8.2/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.8.3/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.8.2/setup.cfg` & `hftbacktest-1.8.3/setup.cfg`

 * *Files identical despite different names*

