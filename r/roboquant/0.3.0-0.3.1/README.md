# Comparing `tmp/roboquant-0.3.0.tar.gz` & `tmp/roboquant-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboquant-0.3.0.tar", last modified: Sat Apr  6 18:16:17 2024, max compression
+gzip compressed data, was "roboquant-0.3.1.tar", last modified: Wed May 29 18:02:25 2024, max compression
```

## Comparing `roboquant-0.3.0.tar` & `roboquant-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,76 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.026627 roboquant-0.3.0/
--rw-r--r--   0 peter      (501) staff       (20)    11341 2024-02-24 08:38:46.000000 roboquant-0.3.0/LICENSE
--rw-r--r--   0 peter      (501) staff       (20)     5705 2024-04-06 18:16:17.026416 roboquant-0.3.0/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     3969 2024-03-26 22:23:08.000000 roboquant-0.3.0/README.md
--rw-r--r--   0 peter      (501) staff       (20)     2207 2024-04-06 09:38:53.000000 roboquant-0.3.0/pyproject.toml
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.014286 roboquant-0.3.0/roboquant/
--rw-r--r--   0 peter      (501) staff       (20)      499 2024-04-06 07:32:58.000000 roboquant-0.3.0/roboquant/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     7367 2024-03-26 09:51:41.000000 roboquant-0.3.0/roboquant/account.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.016070 roboquant-0.3.0/roboquant/brokers/
--rw-r--r--   0 peter      (501) staff       (20)       60 2024-02-24 08:38:46.000000 roboquant-0.3.0/roboquant/brokers/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     5021 2024-03-27 14:00:39.000000 roboquant-0.3.0/roboquant/brokers/alpacabroker.py
--rw-r--r--   0 peter      (501) staff       (20)     2135 2024-03-27 12:19:51.000000 roboquant-0.3.0/roboquant/brokers/broker.py
--rw-r--r--   0 peter      (501) staff       (20)     9249 2024-03-27 13:52:49.000000 roboquant-0.3.0/roboquant/brokers/ibkr.py
--rw-r--r--   0 peter      (501) staff       (20)     9090 2024-03-26 07:55:20.000000 roboquant-0.3.0/roboquant/brokers/simbroker.py
--rw-r--r--   0 peter      (501) staff       (20)      656 2024-03-01 08:16:54.000000 roboquant-0.3.0/roboquant/config.py
--rw-r--r--   0 peter      (501) staff       (20)     5246 2024-03-25 15:12:17.000000 roboquant-0.3.0/roboquant/event.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.019815 roboquant-0.3.0/roboquant/feeds/
--rw-r--r--   0 peter      (501) staff       (20)      510 2024-04-06 09:06:56.000000 roboquant-0.3.0/roboquant/feeds/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     3056 2024-03-15 07:59:42.000000 roboquant-0.3.0/roboquant/feeds/aggregate.py
--rw-r--r--   0 peter      (501) staff       (20)     2459 2024-03-25 22:24:16.000000 roboquant-0.3.0/roboquant/feeds/alpacafeed.py
--rw-r--r--   0 peter      (501) staff       (20)     6474 2024-03-27 06:24:15.000000 roboquant-0.3.0/roboquant/feeds/csvfeed.py
--rw-r--r--   0 peter      (501) staff       (20)     2745 2024-03-03 06:53:49.000000 roboquant-0.3.0/roboquant/feeds/eventchannel.py
--rw-r--r--   0 peter      (501) staff       (20)     3321 2024-04-05 12:09:17.000000 roboquant-0.3.0/roboquant/feeds/feed.py
--rw-r--r--   0 peter      (501) staff       (20)     1712 2024-03-25 13:08:16.000000 roboquant-0.3.0/roboquant/feeds/feedutil.py
--rw-r--r--   0 peter      (501) staff       (20)     2484 2024-03-25 12:56:18.000000 roboquant-0.3.0/roboquant/feeds/historic.py
--rw-r--r--   0 peter      (501) staff       (20)     1082 2024-03-22 06:03:18.000000 roboquant-0.3.0/roboquant/feeds/live.py
--rw-r--r--   0 peter      (501) staff       (20)     2528 2024-03-25 09:27:07.000000 roboquant-0.3.0/roboquant/feeds/randomwalk.py
--rw-r--r--   0 peter      (501) staff       (20)    46215 2024-02-29 18:24:43.000000 roboquant-0.3.0/roboquant/feeds/sp500.json
--rw-r--r--   0 peter      (501) staff       (20)     3275 2024-03-15 07:40:52.000000 roboquant-0.3.0/roboquant/feeds/sqllitefeed.py
--rw-r--r--   0 peter      (501) staff       (20)     9394 2024-03-25 12:30:59.000000 roboquant-0.3.0/roboquant/feeds/tiingo.py
--rw-r--r--   0 peter      (501) staff       (20)     1924 2024-03-17 19:26:05.000000 roboquant-0.3.0/roboquant/feeds/yahoo.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.022263 roboquant-0.3.0/roboquant/journals/
--rw-r--r--   0 peter      (501) staff       (20)      544 2024-02-27 10:15:50.000000 roboquant-0.3.0/roboquant/journals/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     2205 2024-03-09 20:55:00.000000 roboquant-0.3.0/roboquant/journals/alphabeta.py
--rw-r--r--   0 peter      (501) staff       (20)     1082 2024-03-24 15:36:00.000000 roboquant-0.3.0/roboquant/journals/basicjournal.py
--rw-r--r--   0 peter      (501) staff       (20)      859 2024-03-15 22:09:02.000000 roboquant-0.3.0/roboquant/journals/feedmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      833 2024-04-04 07:40:36.000000 roboquant-0.3.0/roboquant/journals/journal.py
--rw-r--r--   0 peter      (501) staff       (20)      478 2024-04-04 07:41:23.000000 roboquant-0.3.0/roboquant/journals/metric.py
--rw-r--r--   0 peter      (501) staff       (20)     1973 2024-03-03 14:18:52.000000 roboquant-0.3.0/roboquant/journals/metricsjournal.py
--rw-r--r--   0 peter      (501) staff       (20)     2057 2024-03-09 20:55:19.000000 roboquant-0.3.0/roboquant/journals/pnlmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      768 2024-02-27 12:20:58.000000 roboquant-0.3.0/roboquant/journals/pricemetric.py
--rw-r--r--   0 peter      (501) staff       (20)      709 2024-02-25 19:17:54.000000 roboquant-0.3.0/roboquant/journals/runmetric.py
--rw-r--r--   0 peter      (501) staff       (20)      996 2024-03-08 14:19:09.000000 roboquant-0.3.0/roboquant/journals/tensorboardjournal.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.023116 roboquant-0.3.0/roboquant/ml/
--rw-r--r--   0 peter      (501) staff       (20)        0 2024-04-06 07:33:32.000000 roboquant-0.3.0/roboquant/ml/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     9034 2024-04-06 07:32:47.000000 roboquant-0.3.0/roboquant/ml/envs.py
--rw-r--r--   0 peter      (501) staff       (20)    14583 2024-03-24 21:59:39.000000 roboquant-0.3.0/roboquant/ml/features.py
--rw-r--r--   0 peter      (501) staff       (20)     9689 2024-04-04 07:32:09.000000 roboquant-0.3.0/roboquant/ml/strategies.py
--rw-r--r--   0 peter      (501) staff       (20)     4477 2024-03-10 08:03:30.000000 roboquant-0.3.0/roboquant/order.py
--rw-r--r--   0 peter      (501) staff       (20)     2142 2024-04-06 09:02:56.000000 roboquant-0.3.0/roboquant/run.py
--rw-r--r--   0 peter      (501) staff       (20)     1500 2024-03-27 16:29:15.000000 roboquant-0.3.0/roboquant/signal.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.024703 roboquant-0.3.0/roboquant/strategies/
--rw-r--r--   0 peter      (501) staff       (20)      232 2024-03-18 17:51:57.000000 roboquant-0.3.0/roboquant/strategies/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     1461 2024-03-27 16:30:10.000000 roboquant-0.3.0/roboquant/strategies/barstrategy.py
--rw-r--r--   0 peter      (501) staff       (20)     2085 2024-03-17 14:29:19.000000 roboquant-0.3.0/roboquant/strategies/buffer.py
--rw-r--r--   0 peter      (501) staff       (20)     2735 2024-04-05 13:37:28.000000 roboquant-0.3.0/roboquant/strategies/emacrossover.py
--rw-r--r--   0 peter      (501) staff       (20)     1718 2024-04-05 13:37:34.000000 roboquant-0.3.0/roboquant/strategies/multistrategy.py
--rw-r--r--   0 peter      (501) staff       (20)     1553 2024-03-27 16:11:34.000000 roboquant-0.3.0/roboquant/strategies/smacrossover.py
--rw-r--r--   0 peter      (501) staff       (20)      652 2024-03-27 15:27:28.000000 roboquant-0.3.0/roboquant/strategies/strategy.py
--rw-r--r--   0 peter      (501) staff       (20)     4354 2024-03-29 08:42:07.000000 roboquant-0.3.0/roboquant/timeframe.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.025600 roboquant-0.3.0/roboquant/traders/
--rw-r--r--   0 peter      (501) staff       (20)       62 2024-02-27 10:15:50.000000 roboquant-0.3.0/roboquant/traders/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     9641 2024-03-27 16:51:27.000000 roboquant-0.3.0/roboquant/traders/flextrader.py
--rw-r--r--   0 peter      (501) staff       (20)     1360 2024-03-21 11:47:01.000000 roboquant-0.3.0/roboquant/traders/sizing.py
--rw-r--r--   0 peter      (501) staff       (20)      967 2024-03-27 16:15:47.000000 roboquant-0.3.0/roboquant/traders/trader.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-04-06 18:16:17.025844 roboquant-0.3.0/roboquant.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)     5705 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     1722 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)      268 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)       25 2024-04-06 18:16:17.000000 roboquant-0.3.0/roboquant.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2024-04-06 18:16:17.026666 roboquant-0.3.0/setup.cfg
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.244788 roboquant-0.3.1/
+-rw-r--r--   0 peter      (501) staff       (20)    11341 2024-02-24 08:38:46.000000 roboquant-0.3.1/LICENSE
+-rw-r--r--   0 peter      (501) staff       (20)     5705 2024-05-29 18:02:25.244589 roboquant-0.3.1/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     3969 2024-04-07 07:47:04.000000 roboquant-0.3.1/README.md
+-rw-r--r--   0 peter      (501) staff       (20)     2207 2024-04-06 09:38:53.000000 roboquant-0.3.1/pyproject.toml
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.236636 roboquant-0.3.1/roboquant/
+-rw-r--r--   0 peter      (501) staff       (20)      516 2024-04-15 08:00:28.000000 roboquant-0.3.1/roboquant/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     7487 2024-05-25 21:25:36.000000 roboquant-0.3.1/roboquant/account.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.237783 roboquant-0.3.1/roboquant/alpaca/
+-rw-r--r--   0 peter      (501) staff       (20)      149 2024-04-14 10:10:59.000000 roboquant-0.3.1/roboquant/alpaca/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     4540 2024-04-13 17:43:23.000000 roboquant-0.3.1/roboquant/alpaca/broker.py
+-rw-r--r--   0 peter      (501) staff       (20)     7207 2024-05-14 09:10:47.000000 roboquant-0.3.1/roboquant/alpaca/feed.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.238335 roboquant-0.3.1/roboquant/brokers/
+-rw-r--r--   0 peter      (501) staff       (20)       60 2024-02-24 08:38:46.000000 roboquant-0.3.1/roboquant/brokers/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     2135 2024-04-07 07:55:14.000000 roboquant-0.3.1/roboquant/brokers/broker.py
+-rw-r--r--   0 peter      (501) staff       (20)     9249 2024-03-27 13:52:49.000000 roboquant-0.3.1/roboquant/brokers/ibkr.py
+-rw-r--r--   0 peter      (501) staff       (20)     9785 2024-05-16 06:29:59.000000 roboquant-0.3.1/roboquant/brokers/simbroker.py
+-rw-r--r--   0 peter      (501) staff       (20)      767 2024-04-10 06:38:52.000000 roboquant-0.3.1/roboquant/config.py
+-rw-r--r--   0 peter      (501) staff       (20)     5468 2024-05-27 07:01:09.000000 roboquant-0.3.1/roboquant/event.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.240483 roboquant-0.3.1/roboquant/feeds/
+-rw-r--r--   0 peter      (501) staff       (20)      499 2024-05-16 17:39:01.000000 roboquant-0.3.1/roboquant/feeds/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     3073 2024-04-10 06:37:57.000000 roboquant-0.3.1/roboquant/feeds/aggregate.py
+-rw-r--r--   0 peter      (501) staff       (20)     4378 2024-05-27 11:55:13.000000 roboquant-0.3.1/roboquant/feeds/avrofeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     1009 2024-04-16 09:17:24.000000 roboquant-0.3.1/roboquant/feeds/collect.py
+-rw-r--r--   0 peter      (501) staff       (20)     6330 2024-05-15 11:42:28.000000 roboquant-0.3.1/roboquant/feeds/csvfeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     2745 2024-04-16 06:54:03.000000 roboquant-0.3.1/roboquant/feeds/eventchannel.py
+-rw-r--r--   0 peter      (501) staff       (20)     3555 2024-05-24 18:14:29.000000 roboquant-0.3.1/roboquant/feeds/feed.py
+-rw-r--r--   0 peter      (501) staff       (20)     2060 2024-05-16 17:38:27.000000 roboquant-0.3.1/roboquant/feeds/feedutil.py
+-rw-r--r--   0 peter      (501) staff       (20)     2719 2024-05-06 07:44:41.000000 roboquant-0.3.1/roboquant/feeds/historic.py
+-rw-r--r--   0 peter      (501) staff       (20)     1346 2024-04-16 11:31:54.000000 roboquant-0.3.1/roboquant/feeds/live.py
+-rw-r--r--   0 peter      (501) staff       (20)     2569 2024-04-10 06:35:51.000000 roboquant-0.3.1/roboquant/feeds/randomwalk.py
+-rw-r--r--   0 peter      (501) staff       (20)    46215 2024-02-29 18:24:43.000000 roboquant-0.3.1/roboquant/feeds/sp500.json
+-rw-r--r--   0 peter      (501) staff       (20)     4786 2024-05-16 17:47:43.000000 roboquant-0.3.1/roboquant/feeds/sqllitefeed.py
+-rw-r--r--   0 peter      (501) staff       (20)     9394 2024-03-25 12:30:59.000000 roboquant-0.3.1/roboquant/feeds/tiingo.py
+-rw-r--r--   0 peter      (501) staff       (20)     1924 2024-03-17 19:26:05.000000 roboquant-0.3.1/roboquant/feeds/yahoo.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.241748 roboquant-0.3.1/roboquant/journals/
+-rw-r--r--   0 peter      (501) staff       (20)      544 2024-02-27 10:15:50.000000 roboquant-0.3.1/roboquant/journals/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     2226 2024-04-13 17:53:37.000000 roboquant-0.3.1/roboquant/journals/alphabeta.py
+-rw-r--r--   0 peter      (501) staff       (20)     1584 2024-05-16 09:19:21.000000 roboquant-0.3.1/roboquant/journals/basicjournal.py
+-rw-r--r--   0 peter      (501) staff       (20)      866 2024-04-13 17:49:14.000000 roboquant-0.3.1/roboquant/journals/feedmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      833 2024-04-04 07:40:36.000000 roboquant-0.3.1/roboquant/journals/journal.py
+-rw-r--r--   0 peter      (501) staff       (20)      478 2024-04-04 07:41:23.000000 roboquant-0.3.1/roboquant/journals/metric.py
+-rw-r--r--   0 peter      (501) staff       (20)     1906 2024-04-13 18:57:30.000000 roboquant-0.3.1/roboquant/journals/metricsjournal.py
+-rw-r--r--   0 peter      (501) staff       (20)     2057 2024-03-09 20:55:19.000000 roboquant-0.3.1/roboquant/journals/pnlmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      768 2024-02-27 12:20:58.000000 roboquant-0.3.1/roboquant/journals/pricemetric.py
+-rw-r--r--   0 peter      (501) staff       (20)      709 2024-02-25 19:17:54.000000 roboquant-0.3.1/roboquant/journals/runmetric.py
+-rw-r--r--   0 peter      (501) staff       (20)     1004 2024-05-18 06:41:05.000000 roboquant-0.3.1/roboquant/journals/tensorboardjournal.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.242263 roboquant-0.3.1/roboquant/ml/
+-rw-r--r--   0 peter      (501) staff       (20)        0 2024-04-06 07:33:32.000000 roboquant-0.3.1/roboquant/ml/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     9250 2024-05-16 14:27:04.000000 roboquant-0.3.1/roboquant/ml/envs.py
+-rw-r--r--   0 peter      (501) staff       (20)    18002 2024-05-16 18:00:06.000000 roboquant-0.3.1/roboquant/ml/features.py
+-rw-r--r--   0 peter      (501) staff       (20)     9649 2024-05-14 15:51:11.000000 roboquant-0.3.1/roboquant/ml/strategies.py
+-rw-r--r--   0 peter      (501) staff       (20)     4504 2024-05-26 10:51:14.000000 roboquant-0.3.1/roboquant/order.py
+-rw-r--r--   0 peter      (501) staff       (20)     2264 2024-04-16 06:56:23.000000 roboquant-0.3.1/roboquant/run.py
+-rw-r--r--   0 peter      (501) staff       (20)     1721 2024-05-16 10:48:43.000000 roboquant-0.3.1/roboquant/signal.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.243094 roboquant-0.3.1/roboquant/strategies/
+-rw-r--r--   0 peter      (501) staff       (20)      230 2024-04-09 20:46:21.000000 roboquant-0.3.1/roboquant/strategies/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     2085 2024-03-17 14:29:19.000000 roboquant-0.3.1/roboquant/strategies/buffer.py
+-rw-r--r--   0 peter      (501) staff       (20)     2749 2024-05-05 10:32:02.000000 roboquant-0.3.1/roboquant/strategies/emacrossover.py
+-rw-r--r--   0 peter      (501) staff       (20)     1773 2024-05-05 10:25:27.000000 roboquant-0.3.1/roboquant/strategies/multistrategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     1567 2024-05-06 08:14:08.000000 roboquant-0.3.1/roboquant/strategies/smacrossover.py
+-rw-r--r--   0 peter      (501) staff       (20)      652 2024-03-27 15:27:28.000000 roboquant-0.3.1/roboquant/strategies/strategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     1473 2024-05-06 07:51:38.000000 roboquant-0.3.1/roboquant/strategies/tastrategy.py
+-rw-r--r--   0 peter      (501) staff       (20)     4664 2024-05-25 21:41:19.000000 roboquant-0.3.1/roboquant/timeframe.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.243713 roboquant-0.3.1/roboquant/traders/
+-rw-r--r--   0 peter      (501) staff       (20)       62 2024-02-27 10:15:50.000000 roboquant-0.3.1/roboquant/traders/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)    10214 2024-05-16 11:17:14.000000 roboquant-0.3.1/roboquant/traders/flextrader.py
+-rw-r--r--   0 peter      (501) staff       (20)     1412 2024-04-15 06:20:22.000000 roboquant-0.3.1/roboquant/traders/sizing.py
+-rw-r--r--   0 peter      (501) staff       (20)      967 2024-03-27 16:15:47.000000 roboquant-0.3.1/roboquant/traders/trader.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2024-05-29 18:02:25.243870 roboquant-0.3.1/roboquant.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)     5705 2024-05-29 18:02:25.000000 roboquant-0.3.1/roboquant.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)     1793 2024-05-29 18:02:25.000000 roboquant-0.3.1/roboquant.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2024-05-29 18:02:25.000000 roboquant-0.3.1/roboquant.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)      268 2024-05-29 18:02:25.000000 roboquant-0.3.1/roboquant.egg-info/requires.txt
+-rw-r--r--   0 peter      (501) staff       (20)       25 2024-05-29 18:02:25.000000 roboquant-0.3.1/roboquant.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)       38 2024-05-29 18:02:25.244836 roboquant-0.3.1/setup.cfg
```

### Comparing `roboquant-0.3.0/LICENSE` & `roboquant-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/PKG-INFO` & `roboquant-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboquant
-Version: 0.3.0
+Version: 0.3.1
 Summary: A fast algo-trading platform
 Author-email: roboquant team <info@roboquant.org>
 Project-URL: Homepage, https://roboquant.org
 Project-URL: Repository, https://github.com/neurallayer/roboquant.py.git
 Project-URL: Issues, https://github.com/neurallayer/roboquant.py/issues
 Keywords: trading,investment,finance,crypto,stocks,exchange,forex
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `roboquant-0.3.0/README.md` & `roboquant-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/pyproject.toml` & `roboquant-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/account.py` & `roboquant-0.3.1/roboquant/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 
     avg_price: float
     """Average price paid denoted in the currency of the symbol"""
 
     mkt_price: float
     """latest market price denoted in the currency of the symbol"""
 
+    @property
+    def is_short(self):
+        return self.size < 0
+
+    @property
+    def is_long(self):
+        return self.size > 0
+
 
 class Converter(ABC):
     """Abstraction that enables trading symbols that are denoted in different currencies and/or contact sizes"""
 
     @abstractmethod
     def __call__(self, symbol: str, time: datetime) -> float:
         """Return the conversion rate for the symbol at the given time"""
@@ -122,15 +130,15 @@
     def contract_value(self, symbol: str, size: Decimal, price: float) -> float:
         # pylint: disable=not-callable
         """Return the total value of the provided contract size denoted in the base currency of the account."""
         rate = 1.0 if not Account.__converter else Account.__converter(symbol, self.last_update)
         return float(size) * price * rate
 
     def mkt_value(self) -> float:
-        """Return the sum of the market values of the open positions in the account.
+        """Return the sum market values of the open positions in the account.
 
         The returned value is denoted in the base currency of the account.
         """
         return sum(
             [self.contract_value(symbol, pos.size, pos.mkt_price) for symbol, pos in self.positions.items()],
             0.0,
         )
@@ -138,16 +146,16 @@
     def position_value(self, symbol) -> float:
         """Return position value denoted in the base currency of the account.
         """
         pos = self.positions.get(symbol)
         return self.contract_value(symbol, pos.size, pos.mkt_price) if pos else 0.0
 
     def equity(self) -> float:
-        """Return the equity of the account. It calcaluates the sum of the mkt value of
-        each open position and adds the available cash.
+        """Return the equity of the account.
+        It calculates the sum mkt values of each open position and adds the available cash.
 
         The returned value is denoted in the base currency of the account.
         """
         return self.cash + self.mkt_value()
 
     def unrealized_pnl(self) -> float:
         """Return the sum of the unrealized profit and loss for the open position.
@@ -176,15 +184,15 @@
         pos = self.positions.get(symbol)
         return pos.size if pos else Decimal(0)
 
     def open_orders(self):
         """Return a list with the open orders"""
         return [order for order in self.orders if order.is_open]
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         p = [f"{v.size}@{k}" for k, v in self.positions.items()]
         p_str = ", ".join(p) or "none"
 
         o = [f"{o.size}@{o.symbol}" for o in self.open_orders()]
         o_str = ", ".join(o) or "none"
 
         result = (
```

### Comparing `roboquant-0.3.0/roboquant/brokers/alpacabroker.py` & `roboquant-0.3.1/roboquant/alpaca/broker.py`

 * *Files 13% similar despite different names*

```diff
@@ -106,27 +106,7 @@
                 symbol=order.symbol, qty=abs(float(order.size)), side=side, time_in_force=TimeInForce.GTC
             )
         return result
 
     def _get_replace_request(self, order: Order):
         result = ReplaceOrderRequest(qty=int(abs(float(order.size))), limit_price=order.limit)
         return result
-
-
-if __name__ == "__main__":
-    broker = AlpacaBroker()
-    account = broker.sync()
-    print(account)
-
-    tsla_order = Order("TSLA", 10)
-    broker.place_orders([tsla_order])
-    time.sleep(5)
-    account = broker.sync()
-    print(account)
-
-    tesla_size = account.get_position_size("TSLA")
-    if tesla_size:
-        tsla_order = Order("TSLA", -tesla_size)
-        broker.place_orders([tsla_order])
-        time.sleep(5)
-        account = broker.sync()
-        print(account)
```

### Comparing `roboquant-0.3.0/roboquant/brokers/broker.py` & `roboquant-0.3.1/roboquant/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/brokers/ibkr.py` & `roboquant-0.3.1/roboquant/brokers/ibkr.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/brokers/simbroker.py` & `roboquant-0.3.1/roboquant/brokers/simbroker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from datetime import timedelta
 from decimal import Decimal
 import logging
 
 from roboquant.account import Account, Position
 from roboquant.brokers.broker import Broker, _update_positions
-from roboquant.event import Event, PriceItem
+from roboquant.event import Event, PriceItem, Quote
 from roboquant.order import Order, OrderStatus
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(slots=True, frozen=True)
 class _Trx:
@@ -82,14 +82,16 @@
                 acc.positions[symbol] = Position(new_size, avg_price, trx.price)
 
     def _get_execution_price(self, order, item) -> float:
         """Return the execution price to use for an order based on the price item.
 
         The default implementation is a fixed slippage percentage based on the configured price_type.
         """
+        if isinstance(item, Quote):
+            return item.ask_price if order.is_buy else item.bid_price
 
         price = item.price(self.price_type)
         correction = self.slippage if order.is_buy else -self.slippage
         return price * (1.0 + correction)
 
     def _execute(self, order: Order, item) -> _Trx | None:
         """Simulate a market execution for the three order types"""
@@ -185,25 +187,40 @@
                         if order.fill == order.size:
                             order.status = OrderStatus.FILLED
 
     def _get_last_known_price(self, symbol):
         item = self._last_known_prices.get(symbol)
         return item.price(self.price_type) if item else None
 
-    def calculate_buyingpower(self):
-        """Calculate buying power, based on the available cash minus the open orders"""
-        bp = self._account.cash
+    def _calculate_open_orders(self):
+        reserved = 0.0
         for order in self._account.open_orders():
             old_pos = self._account.get_position_size(order.symbol)
             remaining = order.size - order.fill
+
+            # only update reserved amount if remaining order size would increase position size
             if abs(old_pos + remaining) > abs(old_pos):
-                price = order.limit or self._get_last_known_price(order.symbol)
-                if price:
-                    reserve = self._account.contract_value(order.symbol, remaining, price)
-                    bp -= abs(reserve)
+                if price := (order.limit or self._get_last_known_price(order.symbol)):
+                    reserved += abs(self._account.contract_value(order.symbol, remaining, price))
+
+        return reserved
+
+    def _calculate_short_positions(self):
+        reserved = 0.0
+        for symbol, position in self._account.positions.items():
+            if position.is_short:
+                short_value = self._account.contract_value(symbol, position.size, position.mkt_price)
+                reserved += abs(short_value)
+        return reserved
+
+    def _calculate_buyingpower(self):
+        """Calculate buying power, based on the available cash minus the open orders and short positions"""
+        bp = self._account.cash
+        bp -= self._calculate_open_orders()
+        bp -= self._calculate_short_positions()
         return bp
 
     def sync(self, event: Event | None = None) -> Account:
         """This will perform the order-execution simulation for the open orders and
         return the updated the account as a result."""
 
         acc = self._account
@@ -219,13 +236,13 @@
             self._create_orders = {order_id: order for order_id, order in self._create_orders.items() if order.is_open}
 
         self._process_modify_order()
         self._process_create_orders(prices)
         _update_positions(acc, event, self.price_type)
 
         acc.orders = list(self._create_orders.values())
-        acc.buying_power = self.calculate_buyingpower()
+        acc.buying_power = self._calculate_buyingpower()
         return acc
 
     def __str__(self) -> str:
         attrs = " ".join([f"{k}={v}" for k, v in self.__dict__.items() if not k.startswith("_")])
         return f"SimBroker({attrs})"
```

### Comparing `roboquant-0.3.0/roboquant/event.py` & `roboquant-0.3.1/roboquant/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,37 @@
     @abstractmethod
     def volume(self, volume_type: str = "DEFAULT") -> float:
         """Return the volume of the price-item"""
 
 
 @dataclass(slots=True)
 class Quote(PriceItem):
-    data: array
+    data: array  # [ask-price, ask-volume, bid-price, bid-volume]
 
     def price(self, price_type: str = "DEFAULT") -> float:
         """Return the price, the default being the mid-point price"""
 
         match price_type:
             case "ASK":
                 return self.data[0]
             case "BID":
                 return self.data[2]
             case _:
                 # Default is the mid-point price
                 return (self.data[0] + self.data[2]) / 2.0
 
     @property
+    def ask_price(self) -> float:
+        return self.data[0]
+
+    @property
+    def bid_price(self) -> float:
+        return self.data[2]
+
+    @property
     def ask_volume(self) -> float:
         return self.data[1]
 
     @property
     def bid_volume(self) -> float:
         return self.data[3]
 
@@ -78,15 +86,15 @@
 
     def volume(self, volume_type: str = "DEFAULT") -> float:
         return self.trade_volume
 
 
 @dataclass(slots=True)
 class Bar(PriceItem):
-    """Represents a bar (a.k.a candlestick) with open, high, low, close and volume data.
+    """Represents a bar (a.k.a. candlestick) with open-, high-, low-, close-price and volume data.
     """
 
     ohlcv: array
     frequency: str = ""  # f.e 1s , 15m, 4h, 1d
 
     @classmethod
     def from_adj_close(cls, symbol, ohlcv: array, adj_close: float, frequency=""):
@@ -126,18 +134,18 @@
         """Return a new empty event"""
 
         time = time or datetime.now(timezone.utc)
         return Event(time, [])
 
     def is_empty(self) -> bool:
         """return True if this is an empty event without any items, False otherwise"""
-        return len(self) == 0
+        return len(self.items) == 0
 
-    def __len__(self) -> int:
-        return len(self.items)
+    # def __len__(self) -> int:
+    #    return len(self.items)
 
     @cached_property
     def price_items(self) -> dict[str, PriceItem]:
         """Returns the price-items in this event for each symbol.
 
         The first time this method is invoked, the result is calculated and cached.
         """
@@ -157,9 +165,9 @@
     def get_volume(self, symbol: str, volume_type: str = "DEFAULT") -> float | None:
         """Return the volume for the symbol, or None if not found."""
 
         if item := self.price_items.get(symbol):
             return item.volume(volume_type)
         return None
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         return f"Event(time={self.time} items={len(self.items)})"
```

### Comparing `roboquant-0.3.0/roboquant/feeds/aggregate.py` & `roboquant-0.3.1/roboquant/feeds/aggregate.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 
 from roboquant.event import Event, Bar, Trade, Quote
 from .eventchannel import EventChannel
 from .feed import Feed
 
 
 class AggregatorFeed(Feed):
-    """Aggregates Trades or Quotes of another feed into a `Bar`.
+    """Aggregates Trades or Quotes of another feed into a `Bar` prices.
 
-    When trades are used, the actual trade price and volume are used to create the aggregated bars.
-    When quotes are used, the midpoint price and no volume are used to create the aggregated bars.
+    When trades are used, the actual trade prices and volumes are used to create the aggregated bars.
+    When quotes are used, the midpoint prices and no volumes are used to create the aggregated bars.
     """
 
     def __init__(
         self,
         feed: Feed,
         frequency: timedelta,
-        item_type: Literal["trade", "quote"] = "trade",
+        price_type: Literal["trade", "quote"] = "trade",
         send_remaining=False,
         continuation=True,
     ):
         super().__init__()
         self.feed = feed
         self.freq = frequency
         self.send_remaining = send_remaining
         self.continuation = continuation
-        self.item_type = item_type
+        self.price_type = price_type
 
     def __aggr_trade2bar(self, evt: Event, bars: dict[str, Bar], freq: str):
 
         for item in evt.items:
 
-            if self.item_type == "trade" and isinstance(item, Trade):
+            if self.price_type == "trade" and isinstance(item, Trade):
                 price = item.trade_price
                 volume = item.trade_volume
-            elif self.item_type == "quote" and isinstance(item, Quote):
+            elif self.price_type == "quote" and isinstance(item, Quote):
                 price = item.midpoint_price
                 volume = float("nan")
             else:
                 continue
 
             symbol = item.symbol
             b = bars.get(symbol)
@@ -55,15 +55,15 @@
             else:
                 bars[symbol] = Bar(symbol, array("f", [price, price, price, price, volume]), freq)
 
     def __get_continued_bars(self, bars: dict[str, Bar]) -> dict[str, Bar]:
         result = {}
         for symbol, item in bars.items():
             p = item.price("CLOSE")
-            v = 0.0 if self.item_type == "trade" else float("nan")
+            v = 0.0 if self.price_type == "trade" else float("nan")
             b = Bar(symbol, array("f", [p, p, p, p, v]))
             result[symbol] = b
         return result
 
     def play(self, channel: EventChannel):
         bars: dict[str, Bar] = {}
         src_channel = self.feed.play_background(channel.timeframe, channel.maxsize)
```

### Comparing `roboquant-0.3.0/roboquant/feeds/csvfeed.py` & `roboquant-0.3.1/roboquant/feeds/csvfeed.py`

 * *Files 11% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     @classmethod
     def stooq_us_daily(cls, path):
         """Parse one or more CSV files that meet the stooq daily file format"""
         columns = ["<DATE>", "<OPEN>", "<HIGH>", "<LOW>", "<CLOSE>", "<VOL>"]
 
         class StooqDailyFeed(CSVFeed):
             def __init__(self):
-                # from Python 3.11 onwards we can use the fast standard ISO parsing
+                # from Python 3.11 onwards, we can use the fast standard ISO parsing
                 if sys.version_info >= (3, 11):
                     super().__init__(path, columns=columns, time_offset="21:00:00+00:00", endswith=".txt", frequency="1d")
                 else:
                     super().__init__(
                         path,
                         columns=columns,
                         time_offset="21:00:00+00:00",
@@ -143,15 +143,15 @@
     @classmethod
     def stooq_us_intraday(cls, path):
         """Parse one or more CSV files that meet the stooq intraday file format"""
         columns = ["<DATE>", "<OPEN>", "<HIGH>", "<LOW>", "<CLOSE>", "<VOL>", "", "<TIME>"]
 
         class StooqIntradayFeed(CSVFeed):
             def __init__(self):
-                # from Python 3.11 onwards we can use the faster standard ISO parsing
+                # from Python 3.11 onwards, we can use the faster standard ISO parsing
                 if sys.version_info >= (3, 11):
                     super().__init__(path, columns=columns, has_time_column=True, endswith=".txt")
                 else:
                     super().__init__(
                         path,
                         columns=columns,
                         has_time_column=True,
@@ -167,15 +167,7 @@
         return StooqIntradayFeed()
 
     @classmethod
     def yahoo(cls, path, frequency="1d"):
         """Parse one or more CSV files that meet the Yahoo Finance format"""
         columns = ["Date", "Open", "High", "Low", "Close", "Volume", "Adj Close"]
         return cls(path, columns=columns, adj_close=True, time_offset="21:00:00+00:00", frequency=frequency)
-
-
-if __name__ == "__main__":
-    t = datetime.strptime("210000", "%H%M%S").time()
-    print(t)
-
-    t = time.fromisoformat("210000")
-    print(t)
```

### Comparing `roboquant-0.3.0/roboquant/feeds/eventchannel.py` & `roboquant-0.3.1/roboquant/feeds/eventchannel.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/feeds/feed.py` & `roboquant-0.3.1/roboquant/feeds/feed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from datetime import datetime
 import threading
 from abc import ABC, abstractmethod
 
 from roboquant.feeds.eventchannel import EventChannel, ChannelClosed
 from roboquant.timeframe import Timeframe
 
+logger = logging.getLogger(__name__)
+
 
 class Feed(ABC):
     """
     A Feed represents a source of (financial) events that can be (re-)played.
     It provides methods for playing events, plotting prices, and playing events in the background on a separate thread.
     """
 
@@ -21,14 +24,15 @@
         ----------
         channel : EventChannel
             EventChannel where the events will be placed.
         """
         ...
 
     def timeframe(self) -> Timeframe | None:
+        """Return the timeframe of this feed it has one and is known, otherwise return None."""
         return None
 
     def play_background(self, timeframe: Timeframe | None = None, channel_capacity: int = 10) -> EventChannel:
         """
         Plays this feed in the background on its own thread.
 
         Parameters
@@ -43,51 +47,50 @@
         EventChannel
             The EventChannel used for playback.
         """
 
         channel = EventChannel(timeframe, channel_capacity)
 
         def __background():
+            # pylint: disable=broad-exception-caught
             try:
                 self.play(channel)
             except ChannelClosed:
                 # this exception we can expect
                 pass
+            except Exception as e:
+                logging.error('Error at playback', exc_info=e)
             finally:
                 channel.close()
 
         thread = threading.Thread(None, __background, daemon=True)
         thread.start()
         return channel
 
     def plot(self, plt, symbol: str, price_type: str = "DEFAULT", timeframe: Timeframe | None = None, **kwargs):
         """
         Plot the prices of a symbol.
 
         Parameters
         ----------
-        plt : matplotlib.pyplot
+        plt : matplotlib axes
             The matplotlib.pyplot object where the plot will be drawn.
         symbol : str
             The symbol for which to plot prices.
         price_type : str, optional
             The type of price to plot, e.g. open, close, high, low. (default is "DEFAULT")
         timeframe : Timeframe or None, optional
             The timeframe over which to plot prices. If None, the entire feed timeframe is used. (default is None)
         **kwargs
             Additional keyword arguments to pass to the plt.plot() function.
         """
-
+        plt = plt.subplot() if hasattr(plt, "subplot") else plt
         times, prices = get_symbol_prices(self, symbol, price_type, timeframe)
         plt.plot(times, prices, **kwargs)
-        if hasattr(plt, "set_title"):
-            # assume we are in a subplot
-            plt.set_title(symbol)
-        else:
-            plt.title(symbol)
+        plt.set_title(symbol)
 
 
 def get_symbol_prices(
         feed: Feed, symbol: str, price_type="DEFAULT", timeframe: Timeframe | None = None
 ) -> tuple[list[datetime], list[float]]:
     """Get prices for a single symbol from a feed"""
```

### Comparing `roboquant-0.3.0/roboquant/feeds/feedutil.py` & `roboquant-0.3.1/roboquant/feeds/feedutil.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,7 +41,18 @@
     """
 
     channel = feed.play_background(timeframe)
     while event := channel.get(timeout):
         print(event.time)
         for item in event.items:
             print("======> ", item)
+
+
+def count_events(feed: Feed, timeframe: Timeframe | None = None, timeout: float | None = None, include_empty=False):
+    """Count the number of events in a feed"""
+
+    channel = feed.play_background(timeframe)
+    events = 0
+    while evt := channel.get(timeout):
+        if evt.items or include_empty:
+            events += 1
+    return events
```

### Comparing `roboquant-0.3.0/roboquant/feeds/historic.py` & `roboquant-0.3.1/roboquant/feeds/historic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from datetime import datetime
 from itertools import chain
 from typing import List
 
 from roboquant.event import Event, PriceItem
-from roboquant.timeframe import Timeframe
+from roboquant.timeframe import EMPTY_TIMEFRAME, Timeframe
 from .eventchannel import EventChannel
 from .feed import Feed
 from .feedutil import get_ohlcv
 
 
 class HistoricFeed(Feed, ABC):
     """
@@ -18,15 +18,20 @@
     def __init__(self):
         super().__init__()
         self.__data: dict[datetime, list[PriceItem]] = {}
         self.__modified = False
         self.__symbols = []
 
     def _add_item(self, time: datetime, item: PriceItem):
-        """Add a price-item at a moment in time to this feed"""
+        """Add a price-item at a moment in time to this feed.
+        Subclasses should invoke this method to populate the historic-feed.
+
+        Items added at the same time, will be part of the same event.
+        So each unique time will only produce a single event.
+        """
 
         self.__modified = True
 
         if time not in self.__data:
             self.__data[time] = [item]
         else:
             items = self.__data[time]
@@ -34,26 +39,31 @@
 
     @property
     def symbols(self):
         """Return the list of unique symbols available in this feed"""
         self.__update()
         return self.__symbols
 
+    @property
+    def events(self):
+        """Return the total number of events"""
+        return len(self.__data)
+
     def timeline(self) -> List[datetime]:
         """Return the timeline of this feed as a list of datatime objects"""
         self.__update()
         return list(self.__data.keys())
 
     def timeframe(self):
         """Return the timeframe of this feed"""
         tl = self.timeline()
-        if not tl:
-            raise ValueError("Feed doesn't contain any events.")
+        if tl:
+            return Timeframe(tl[0], tl[-1], inclusive=True)
 
-        return Timeframe(tl[0], tl[-1], inclusive=True)
+        return EMPTY_TIMEFRAME
 
     def get_ohlcv(self, symbol: str, timeframe=None) -> dict[str, list]:
         """Get the OHLCV values for a symbol for the (optional) provided timeframe.
         This makes it easy to plot prices and use them in a dataframe.
         """
         return get_ohlcv(self, symbol, timeframe)
 
@@ -66,12 +76,10 @@
 
     def play(self, channel: EventChannel):
         self.__update()
         for k, v in self.__data.items():
             evt = Event(k, v)
             channel.put(evt)
 
-    def __repr__(self) -> str:
-        events = len(self.timeline())
-        timeframe = self.timeframe() if events else None
+    def __str__(self) -> str:
         feed = self.__class__.__name__
-        return f"{feed}(events={events} symbols={len(self.symbols)} timeframe={timeframe})"
+        return f"{feed}(events={self.events} symbols={len(self.symbols)} timeframe={self.timeframe()})"
```

### Comparing `roboquant-0.3.0/roboquant/feeds/live.py` & `roboquant-0.3.1/roboquant/feeds/live.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 from .feed import Feed
 
 
 class LiveFeed(Feed):
     """
     Abstract base class for feeds that produce live price-items. It will ensure that
     events that are published are monotonic in time (so always increasing).
+
+    If a new event has a timestamp that is before or equal to the previous event, the
+    timstamp will be corrected so the event occurs after the previous event.
+
+    The default is to increment it by 1 microsecond over the previous event, but this is configurable.
     """
 
     def __init__(self):
         super().__init__()
         self._channel = None
         self._last_time = datetime.fromisoformat("1900-01-01T00:00:00+00:00")
-        self._min_change = timedelta(microseconds=1)
+        self.increment = timedelta(microseconds=1)
 
     def play(self, channel: EventChannel):
         self._channel = channel
         while not channel.is_closed:
             time.sleep(1)
         self._channel = None
 
     def put(self, event: Event):
         if self._channel:
             try:
                 if event.time <= self._last_time:
-                    event.time = self._last_time + self._min_change
+                    event.time = self._last_time + self.increment
                 self._channel.put(event)
                 self._last_time = event.time
             except ChannelClosed:
                 pass
```

### Comparing `roboquant-0.3.0/roboquant/feeds/randomwalk.py` & `roboquant-0.3.1/roboquant/feeds/randomwalk.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import numpy as np
 
 from roboquant.event import Bar, Trade
 from .historic import HistoricFeed
 
 
 class RandomWalk(HistoricFeed):
-    """This feed simulates the random-walk of stock prices."""
+    """This feed simulates the random-walk of stock prices.
+    It can generate trade or bar prices."""
 
     def __init__(
         self,
         n_symbols: int = 10,
         n_prices: int = 1_000,
         item_type: Literal["bar", "trade"] = "bar",
         start_date: str | datetime = "2020-01-01T00:00:00+00:00",
```

### Comparing `roboquant-0.3.0/roboquant/feeds/sp500.json` & `roboquant-0.3.1/roboquant/feeds/sp500.json`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/feeds/tiingo.py` & `roboquant-0.3.1/roboquant/feeds/tiingo.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/feeds/yahoo.py` & `roboquant-0.3.1/roboquant/feeds/yahoo.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/__init__.py` & `roboquant-0.3.1/roboquant/journals/__init__.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/alphabeta.py` & `roboquant-0.3.1/roboquant/journals/alphabeta.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class AlphaBeta(Metric):
     """
     Calculate the alpha and beta.
     """
 
-    def __init__(self, window_size, price_type="DEFAULT", risk_free_return=0.0):
+    def __init__(self, window_size: int, price_type: str = "DEFAULT", risk_free_return: float = 0.0):
         """
         window_size: the rolling window_size to use. The alpha and beta are only calculated once the window is filled.
         price_type: the type of price to use to calculate the market returns, default is "DEFAULT"
         risk_free_return: the risk-free return rate, default is 0.0
         """
 
         # data stores both portfolio return and market return
```

### Comparing `roboquant-0.3.0/roboquant/journals/feedmetric.py` & `roboquant-0.3.1/roboquant/journals/feedmetric.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from roboquant.journals.metric import Metric
 
 
 class FeedMetric(Metric):
-    """Tracks the combined performance of the price-items in the event"""
+    """Tracks the performance of the market, aka the price-items in the event"""
 
     def __init__(self, price_type="DEFAULT"):
         self._prev_prices = {}
         self.price_type = price_type
         self._last_total = 1.0
 
     def calc(self, event, account, signals, orders):
```

### Comparing `roboquant-0.3.0/roboquant/journals/journal.py` & `roboquant-0.3.1/roboquant/journals/journal.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/metricsjournal.py` & `roboquant-0.3.1/roboquant/journals/metricsjournal.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,24 +38,22 @@
                 timeline.append(time)
                 values.append(metrics[metric_name])
         return timeline, values
 
     def plot(self, plt, metric_name: str, plot_x: bool = True, **kwargs):
         """Plot a metric"""
         x, y = self.get_timeseries(metric_name)
+        plt = plt.subplot() if hasattr(plt, "subplot") else plt
+
         if plot_x:
             plt.plot(x, y, **kwargs)
         else:
             plt.plot(y, **kwargs)
 
-        if hasattr(plt, "set_title"):
-            # assume we are in a subplot
-            plt.set_title(metric_name)
-        else:
-            plt.title(metric_name)
+        plt.set_title(metric_name)
 
     def get_metric_names(self) -> set[str]:
         """return the available metric names in this journal"""
         result = set()
         for _, m in self._history:
             result.update(m.keys())
         return result
```

### Comparing `roboquant-0.3.0/roboquant/journals/pnlmetric.py` & `roboquant-0.3.1/roboquant/journals/pnlmetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/pricemetric.py` & `roboquant-0.3.1/roboquant/journals/pricemetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/runmetric.py` & `roboquant-0.3.1/roboquant/journals/runmetric.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/journals/tensorboardjournal.py` & `roboquant-0.3.1/roboquant/journals/tensorboardjournal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from roboquant.journals import Journal
+from roboquant.journals.journal import Journal
 from roboquant.journals.metric import Metric
 
 
 class TensorboardJournal(Journal):
     """Record metrics to a Tensorboard compatible file.
 
     This can be used outside the realm of machine learning, but requires tensorboard to be installed.
```

### Comparing `roboquant-0.3.0/roboquant/ml/envs.py` & `roboquant-0.3.1/roboquant/ml/envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from decimal import Decimal
 import logging
 import gymnasium as gym
 from gymnasium import spaces
 from gymnasium.envs.registration import register
 import numpy as np
 from numpy.typing import NDArray
@@ -29,15 +30,17 @@
     """Transforms an action into signals"""
 
     def __init__(self, symbols: list[str]):
         self.symbols = symbols
 
     @staticmethod
     def __limit(rating):
-        return max(-1.0, min(1.0, float(rating)))
+        rating = float(rating)
+        assert math.isfinite(rating), f"rating not finite rating={rating}"
+        return max(-1.0, min(1.0, rating))
 
     def get_signals(self, action, _):
         return [Signal(symbol, self.__limit(rating)) for symbol, rating in zip(self.symbols, action)]
 
     def get_action_space(self):
         return spaces.Box(-1.0, 1.0, shape=(len(self.symbols),), dtype=np.float32)
 
@@ -108,15 +111,15 @@
         self.observation_space = spaces.Box(-1.0, 1.0, shape=(self.obs_feature.size(),), dtype=np.float32)
         self.action_space = action_2_signals.get_action_space()
         logger.info("observation_space=%s action_space=%s", self.observation_space, self.action_space)
 
     def get_observation(self, evt: Event) -> NDArray[np.float32]:
         return self.obs_feature.calc(evt, None)
 
-    def get_reward(self, evt: Event, account: Account):
+    def get_reward(self, evt: Event, account: Account) -> NDArray[np.float32]:
         return self.reward_feature.calc(evt, account)
 
     def step(self, action):
         assert self.event is not None
         assert self.account is not None
         signals = self.action_2_signals.get_signals(action, self.event)
         logger.debug("time=%s signals=%s", self.event.time, signals)
@@ -131,14 +134,15 @@
             reward = self.get_reward(self.event, self.account)
             return observation, reward, False, False, {}
 
         return None, 0.0, True, False, {}
 
     def reset(self, *, seed=None, options=None):
         super().reset(seed=seed, options=options)
+        logger.info("environment resetting")
         self.broker.reset()
         self.trader.reset()
         self.obs_feature.reset()
         self.reward_feature.reset()
 
         self.channel = self.feed.play_background(self.timeframe)
 
@@ -231,14 +235,15 @@
             self.event = self.channel.get()
             assert self.event is not None, "feed empty during warmup"
             self.account = self.broker.sync(self.event)
             observation = self.get_observation(self.event, self.account)
             self.get_reward(self.event, self.account)
             if not np.any(np.isnan(observation)):
                 return observation, {}
+            logger.info(observation)
 
     def render(self):
         pass
 
     def __str__(self):
         result = (
             f"TradingEnv(\n\tbroker={self.broker}\n\tfeed={self.feed}"
```

### Comparing `roboquant-0.3.0/roboquant/ml/features.py` & `roboquant-0.3.1/roboquant/ml/features.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,88 @@
 from abc import ABC, abstractmethod
 from collections import deque
 from datetime import datetime, timezone
+from typing import Any
 
 import numpy as np
 from numpy.typing import NDArray
 
 from roboquant.account import Account
-from roboquant.event import Event, Bar
+from roboquant.event import Event, Bar, Quote
+from roboquant.strategies.buffer import OHLCVBuffer
 
 
 class Feature(ABC):
     """Features allows to:
     - extract features from an event and/or account.
     - transform other features.
     """
 
     @abstractmethod
     def calc(self, evt: Event, account: Account | None) -> NDArray:
         """
         Return the result as a 1-dimensional NDArray.
-        The result should always be the same size.
+        The result should always be the same size. If a value cannot be calculated at a certain
+        tiem, it should return a float NaN.
         """
 
     @abstractmethod
     def size(self) -> int:
-        "return the size of this feature"
+        """return the size of this feature"""
 
-    def shape(self):
+    def _shape(self):
+        """return the shape of this feature as a tuple"""
         return (self.size(),)
 
     def returns(self, period=1):
         if period == 1:
             return ReturnsFeature(self)
         return LongReturnsFeature(self, period)
 
     def normalize(self, min_period=3):
         return NormalizeFeature(self, min_period)
 
-    def cache(self):
-        return CacheFeature(self)
+    def cache(self, validate=False):
+        return CacheFeature(self, validate)
 
     def __getitem__(self, *args):
         return SlicedFeature(self, args)
 
     def reset(self):
         """Reset the state of the feature"""
 
     def _zeros(self):
-        return np.zeros(self.shape(), dtype=np.float32)
+        return np.zeros(self._shape(), dtype=np.float32)
 
     def _ones(self):
-        return np.ones(self.shape(), dtype=np.float32)
+        return np.ones(self._shape(), dtype=np.float32)
 
     def _full_nan(self):
-        return np.full(self.shape(), float("nan"), dtype=np.float32)
+        return np.full(self._shape(), float("nan"), dtype=np.float32)
 
 
 class SlicedFeature(Feature):
+    """Calculate a slice from another feature"""
 
     def __init__(self, feature: Feature, args) -> None:
         super().__init__()
         self.args = args
         self.feature = feature
         self._size = len(feature._zeros()[args])
 
     def calc(self, evt, account):
         values = self.feature.calc(evt, account)
         return values[self.args]
 
     def size(self):
         return self._size
 
+    def reset(self):
+        return self.feature.reset()
+
 
 class TrueRangeFeature(Feature):
     """Calculates the true range value for a symbol"""
 
     def __init__(self, symbol: str) -> None:
         super().__init__()
         self.prev_close = None
@@ -102,17 +110,17 @@
 
     def reset(self):
         self.prev_close = None
 
 
 class FixedValueFeature(Feature):
 
-    def __init__(self, value: NDArray) -> None:
+    def __init__(self, value: Any) -> None:
         super().__init__()
-        self.value = value
+        self.value = np.array(value, dtype="float32")
 
     def size(self) -> int:
         return len(self.value)
 
     def calc(self, evt, account):
         return self.value
 
@@ -142,37 +150,38 @@
         return np.asarray([equity], dtype=np.float32)
 
     def size(self) -> int:
         return 1
 
 
 class PositionSizeFeature(Feature):
-    """Extract the position value for a symbol as fraction of the total equity"""
+    """Extract the position value for one or more symbols as the fraction of the total equity"""
 
     def __init__(self, *symbols: str) -> None:
         super().__init__()
         self.symbols = symbols
 
     def calc(self, evt, account):
         assert account is not None
         result = self._zeros()
+        equity = account.equity()
         for idx, symbol in enumerate(self.symbols):
             position = account.positions.get(symbol)
             if position:
                 value = account.contract_value(symbol, position.size, position.mkt_price)
-                pos_size = value / account.equity() - 1.0
+                pos_size = value / equity - 1.0
                 result[idx] = pos_size
         return result
 
     def size(self) -> int:
         return len(self.symbols)
 
 
 class PositionPNLFeature(Feature):
-    """Extract the pnl for an open position for a symbol.
+    """Extract the pnl percentage for an open position for one or more symbols.
     Returns 0.0 if there is no open position for a symbol"""
 
     def __init__(self, *symbols: str) -> None:
         super().__init__()
         self.symbols = symbols
 
     def calc(self, evt, account):
@@ -206,14 +215,35 @@
 
         return result
 
     def size(self) -> int:
         return 5 * len(self.symbols)
 
 
+class QuoteFeature(Feature):
+    """Extract the values from quotes for one or more symbols"""
+
+    def __init__(self, *symbols: str) -> None:
+        super().__init__()
+        self.symbols = symbols
+
+    def calc(self, evt, account):
+        result = self._full_nan()
+        for idx, symbol in enumerate(self.symbols):
+            item = evt.price_items.get(symbol)
+            if isinstance(item, Quote):
+                offset = idx * 4
+                result[offset: offset + 4] = item.data
+
+        return result
+
+    def size(self) -> int:
+        return 4 * len(self.symbols)
+
+
 class CombinedFeature(Feature):
     """Combine multiple features into one single feature by stacking them."""
 
     def __init__(self, *features: Feature) -> None:
         super().__init__()
         self.features = features
         self._size = sum(feature.size() for feature in self.features)
@@ -221,14 +251,18 @@
     def calc(self, evt, account):
         data = [feature.calc(evt, account) for feature in self.features]
         return np.hstack(data, dtype=np.float32)
 
     def size(self) -> int:
         return self._size
 
+    def reset(self):
+        for feature in self.features:
+            feature.reset()
+
 
 class NormalizeFeature(Feature):
     """online normalization calculator"""
 
     def __init__(self, feature: Feature, min_count: int = 3) -> None:
         super().__init__()
         self.feature = feature
@@ -241,15 +275,15 @@
     def denormalize(self, value):
         (count, mean, m2) = self.existing_aggregate
         stdev = np.sqrt(m2 / count) - 1e-12
         return value * stdev + mean
 
     def __update(self, new_value):
         (count, mean, m2) = self.existing_aggregate
-        mask = ~ np.isnan(new_value)
+        mask = ~np.isnan(new_value)
         count[mask] += 1
         delta = new_value - mean
         mean[mask] += delta[mask] / count[mask]
         delta2 = new_value - mean
         m2[mask] += delta[mask] * delta2[mask]
 
     def __normalize_values(self, values):
@@ -265,14 +299,15 @@
         return self.__normalize_values(values)
 
     def size(self) -> int:
         return self.feature.size()
 
     def reset(self):
         self.existing_aggregate = (self._zero_int(), self._zeros(), self._zeros())
+        self.feature.reset()
 
 
 class FillFeature(Feature):
     """If a feature contains a nan value, use the last known value instead"""
 
     def __init__(self, feature: Feature) -> None:
         super().__init__()
@@ -291,55 +326,62 @@
         self.feature.reset()
 
     def size(self) -> int:
         return self.feature.size()
 
 
 class CacheFeature(Feature):
-    """Cache the results of a feature. This requires the feed to have always increasing time value
-    and the feature to produce same output.
+    """Cache the results of a feature. This requires the feed to have an always increasing time value
+    and the feature to produce the same output at a given time.
 
-    Typically this doesn't work for features that depend on account values.
+    Typically, this doesn't work for features that depend on account values.
     """
 
-    def __init__(self, feature: Feature) -> None:
+    def __init__(self, feature: Feature, validate=False) -> None:
         super().__init__()
         self.feature: Feature = feature
         self._cache: dict[datetime, NDArray] = {}
+        self.validate = validate
 
     def calc(self, evt, account):
         time = evt.time
         if time in self._cache:
-            return self._cache[time]
+            values = self._cache[time]
+            if self.validate:
+                calc_values = self.feature.calc(evt, account)
+                assert np.array_equal(
+                    values, calc_values, equal_nan=True
+                ), f"Wrong cache time={time} cache={values} calculated={calc_values}"
+            return values
 
         values = self.feature.calc(evt, account)
         self._cache[time] = values
         return values
 
     def reset(self):
-        """Reset the underlying feature. This doesn't cleear the cache"""
+        """Reset the underlying feature. This doesn't clear the cache"""
         self.feature.reset()
 
     def clear(self):
-        """Clear all of the cache"""
+        """Clear all the cache"""
         self._cache = {}
 
     def size(self) -> int:
         return self.feature.size()
 
 
 class VolumeFeature(Feature):
     """Extract the volume for one or more symbols"""
 
     def __init__(self, *symbols: str, volume_type: str = "DEFAULT") -> None:
         super().__init__()
         self.symbols = symbols
         self.volume_type = volume_type
 
-    def calc(self, evt: Event, account: Account):
+    def calc(self, evt: Event, account):
         volumes = [evt.get_volume(symbol, self.volume_type) for symbol in self.symbols]
         return np.array(volumes, dtype=np.float32)
 
     def size(self) -> int:
         return len(self.symbols)
 
 
@@ -394,14 +436,15 @@
 class MaxReturnFeature(Feature):
     """Calculate the maximum return over a certain period.
     This will only work on features that return a single value.
     """
 
     def __init__(self, feature: Feature, period: int) -> None:
         super().__init__()
+        assert feature.size() == 1
         self.history = deque(maxlen=period)
         self.feature: Feature = feature
 
     def calc(self, evt, account):
         values = self.feature.calc(evt, account)
         h = self.history
 
@@ -418,16 +461,15 @@
 
     def reset(self):
         self.history.clear()
         self.feature.reset()
 
 
 class MaxReturnFeature2(Feature):
-    """Calculate the maximum return over a certain period.
-    """
+    """Calculate the maximum return over a certain period."""
 
     def __init__(self, feature: Feature, period: int) -> None:
         super().__init__()
         self.feature: Feature = feature
         self.history = np.full((period, self.size()), float("nan"), dtype=np.float32)
         self.idx = -1
 
@@ -509,24 +551,88 @@
 
     def size(self) -> int:
         return self.feature.size()
 
     def reset(self):
         self.history = None
         self.feature.reset()
+        self._cnt = 0
 
 
 class DayOfWeekFeature(Feature):
-    """Calculate a one-hot-encoded day of the week, Monday being 0"""
+    """Calculate a one-hot-encoded day of the week where Monday == 0 and Sunday == 6"""
 
     def __init__(self, tz=timezone.utc) -> None:
+        super().__init__()
         self.tz = tz
 
     def calc(self, evt, account):
         dt = datetime.astimezone(evt.time, self.tz)
         weekday = dt.weekday()
         result = np.zeros(7, dtype=np.float32)
         result[weekday] = 1.0
         return result
 
     def size(self) -> int:
         return 7
+
+
+class TimeDifference(Feature):
+    """Calculate the time difference in seconds between two consecutive events."""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._last_time: datetime | None = None
+
+    def calc(self, evt, account):
+        if self._last_time:
+            diff = evt.time - self._last_time
+            self._last_time = evt.time
+            return np.asarray([diff.total_seconds()], dtype="float32")
+
+        self._last_time = evt.time
+        return self._full_nan()
+
+    def size(self) -> int:
+        return 1
+
+    def reset(self):
+        self._last_time = None
+
+
+class TaFeature(Feature):
+    """Base class for technical analysis features"""
+
+    def __init__(self, *symbols: str, history_size: int) -> None:
+        super().__init__()
+        self._data: dict[str, OHLCVBuffer] = {}
+        self._size = history_size
+        self.symbols = list(symbols)
+
+    def calc(self, evt, account):
+        result = []
+        nan = float("nan")
+        for symbol in self.symbols:
+            value = nan
+            item = evt.price_items.get(symbol)
+            if isinstance(item, Bar):
+                symbol = item.symbol
+                if symbol not in self._data:
+                    self._data[symbol] = OHLCVBuffer(self._size)
+                ohlcv = self._data[symbol]
+                ohlcv.append(item.ohlcv)
+                if ohlcv.is_full():
+                    value = self._calc(symbol, ohlcv)
+
+            result.append(value)
+        return np.asarray(result, dtype=np.float32)
+
+    @abstractmethod
+    def _calc(self, symbol: str, ohlcv: OHLCVBuffer) -> float:
+        """Override this method with technical analysis logic"""
+        ...
+
+    def size(self) -> int:
+        return len(self.symbols)
+
+    def reset(self):
+        self._data = {}
```

### Comparing `roboquant-0.3.0/roboquant/ml/strategies.py` & `roboquant-0.3.1/roboquant/ml/strategies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import abstractmethod
 from collections import deque
+from datetime import datetime
 import logging
 import numpy as np
 from numpy.typing import NDArray
 from stable_baselines3.common.policies import BasePolicy
 import torch
 from torch.utils.data import DataLoader, Dataset
 
@@ -30,16 +31,17 @@
     @classmethod
     def from_env(cls, env: StrategyEnv, policy):
         return cls(env.obs_feature, env.action_2_signals, policy)
 
     def create_signals(self, event):
         obs = self.obs_feature.calc(event, None)
         if np.any(np.isnan(obs)):
-            return {}
+            return []
         action, self.state = self.policy.predict(obs, state=self.state, deterministic=True)  # type: ignore
+        logger.debug(action)
         return self.action_2_signals.get_signals(action, event)
 
     def reset(self):
         self.state = None
         self.obs_feature.reset()
 
 
@@ -52,66 +54,49 @@
         self.policy = policy
         self.state = None
 
     @classmethod
     def from_env(cls, env: TraderEnv, policy):
         return cls(env.obs_feature, env.action_2_orders, policy)
 
-    def create_orders(self, _, event, account) -> list[Order]:
+    def create_orders(self, signals, event, account) -> list[Order]:
         obs = self.obs_feature.calc(event, account)
         if np.any(np.isnan(obs)):
             return []
         action, self.state = self.policy.predict(obs, state=self.state, deterministic=True)  # type: ignore
         return self.action_2_orders.get_orders(action, event, account)
 
     def reset(self):
         super().reset()
         self.state = None
         self.obs_feature.reset()
 
 
 class FeatureStrategy(Strategy):
     """Abstract base class for strategies wanting to use features
-    for their input and target.
+    for their input.
     """
 
-    def __init__(self, input_feature: Feature, label_feature: Feature, history: int, dtype="float32"):
-        self._features_x = []
-        self._features_y = []
+    def __init__(self, input_feature: Feature, history: int, dtype="float32"):
         self.input_feature = input_feature
-        self.label_feature = label_feature
+        self.history = history
         self._hist = deque(maxlen=history)
         self._dtype = dtype
 
     def create_signals(self, event: Event):
         h = self._hist
         row = self.input_feature.calc(event, None)
         h.append(row)
         if len(h) == h.maxlen:
             x = np.asarray(h, dtype=self._dtype)
-            return self.predict(x)
+            return self.predict(x, event.time)
         return []
 
     @abstractmethod
-    def predict(self, x: NDArray) -> list[Signal]: ...
-
-    def _get_xy(self, feed, timeframe=None, warmup=0) -> tuple[NDArray, NDArray]:
-        channel = feed.play_background(timeframe)
-        x = []
-        y = []
-        while evt := channel.get():
-            if warmup:
-                self.label_feature.calc(evt, None)
-                self.input_feature.calc(evt, None)
-                warmup -= 1
-            else:
-                x.append(self.input_feature.calc(evt, None))
-                y.append(self.label_feature.calc(evt, None))
-
-        return np.asarray(x, dtype=self._dtype), np.asarray(y, dtype=self._dtype)
+    def predict(self, x: NDArray, time: datetime) -> list[Signal]: ...
 
 
 class SequenceDataset(Dataset):
     """Sequence Dataset"""
 
     def __init__(self, x_data: NDArray, y_data: NDArray, sequences=20, transform=None, target_transform=None):
         self.sequences = sequences
@@ -142,62 +127,76 @@
         label_feature: Feature,
         model: torch.nn.Module,
         symbol: str,
         sequences: int = 20,
         buy_pct: float = 0.01,
         sell_pct=0.0,
     ):
-        super().__init__(input_feature, label_feature, sequences)
-        self.sequences = sequences
+        super().__init__(input_feature, sequences)
+        self.label_feature = label_feature
         self.model = model
         self.buy_pct = buy_pct
         self.sell_pct = sell_pct
         self.symbol = symbol
-        self.prediction_results = []
 
-    def predict(self, x):
+    def predict(self, x, time):
         x = torch.asarray(x)
         x = torch.unsqueeze(x, dim=0)  # add the batch dimension
 
         self.model.eval()
         with torch.no_grad():
             output = self.model(x).numpy()
 
             if isinstance(self.label_feature, NormalizeFeature):
                 p = self.label_feature.denormalize(output).item()
             else:
                 p = output.item()
 
-            self.prediction_results.append(p)
+            logger.info("prediction p=%s time=%s", p, time)
             if p >= self.buy_pct:
                 return [Signal.buy(self.symbol)]
             if p <= self.sell_pct:
                 return [Signal.sell(self.symbol)]
 
-        return {}
+        return []
 
     def _get_dataloaders(self, x, y, prediction: int, validation_split: float, batch_size: int):
         # what is the border between train- and validation-data
         border = round(len(y) * (1.0 - validation_split))
 
         x_train = x[: border - prediction]
         y_train = y[prediction:border]
 
-        train_dataset = SequenceDataset(x_train, y_train, self.sequences)
+        train_dataset = SequenceDataset(x_train, y_train, self.history)
         train_dataloader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
 
         valid_dataloader = None
         if validation_split > 0.0:
             x_valid = x[border - prediction: -prediction]
             y_valid = y[border:]
-            valid_dataset = SequenceDataset(x_valid, y_valid, self.sequences)
+            valid_dataset = SequenceDataset(x_valid, y_valid, self.history)
             valid_dataloader = DataLoader(valid_dataset, batch_size=batch_size, shuffle=False)
 
         return train_dataloader, valid_dataloader
 
+    def __get_xy(self, feed, timeframe=None, warmup=0) -> tuple[NDArray, NDArray]:
+        channel = feed.play_background(timeframe)
+        x = []
+        y = []
+        while evt := channel.get():
+            if warmup:
+                self.label_feature.calc(evt, None)
+                self.input_feature.calc(evt, None)
+                warmup -= 1
+            else:
+                x.append(self.input_feature.calc(evt, None))
+                y.append(self.label_feature.calc(evt, None))
+
+        return np.asarray(x, dtype=self._dtype), np.asarray(y, dtype=self._dtype)
+
     @staticmethod
     def describe(x):
         print("shape=", x.shape, "min=", np.min(x, axis=0), "max=", np.max(x, axis=0), "mean=", np.mean(x, axis=0))
 
     def fit(
         self,
         feed,
@@ -225,15 +224,15 @@
             batch_size: The batch size to use, default is 32.
             validation_split: the percentage to use for validation, default is 0.20 (20%).
             writer: the tensorboard writer to use to log losses, default is None.
         """
         optimizer = optimizer or torch.optim.Adam(self.model.parameters(), lr=0.001)
         criterion = criterion or torch.nn.MSELoss()
 
-        x, y = self._get_xy(feed, timeframe, warmup=warmup)
+        x, y = self.__get_xy(feed, timeframe, warmup=warmup)
         logger.info("x-shape=%s", x.shape)
         logger.info("y-shape=%s", y.shape)
 
         train_dataloader, valid_dataloader = self._get_dataloaders(x, y, prediction, validation_split, batch_size)
 
         for epoch in range(epochs):
             train_loss = self._train_epoch(train_dataloader, optimizer, criterion)
```

### Comparing `roboquant-0.3.0/roboquant/order.py` & `roboquant-0.3.1/roboquant/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,24 @@
     CANCELLED = auto()
     EXPIRED = auto()
 
     _OPEN = INITIAL | ACTIVE
     _CLOSE = REJECTED | FILLED | CANCELLED | EXPIRED
 
     @property
-    def open(self):
+    def is_open(self):
         """Return True is the status is open, False otherwise"""
         return self in OrderStatus._OPEN
 
     @property
-    def closed(self):
+    def is_closed(self):
         """Return True is the status is closed, False otherwise"""
         return self in OrderStatus._CLOSE
 
-    def __repr__(self):
+    def __str__(self):  # type: ignore
         return self.name
 
 
 @dataclass(slots=True)
 class Order:
     """
     A trading order.
@@ -73,20 +73,20 @@
         self.status: OrderStatus = OrderStatus.INITIAL
         self.fill = Decimal(0)
         self.info = kwargs
 
     @property
     def is_open(self) -> bool:
         """Return True is the order is open, False otherwise"""
-        return self.status.open
+        return self.status.is_open
 
     @property
     def is_closed(self) -> bool:
         """Return True is the order is closed, False otherwise"""
-        return self.status.closed
+        return self.status.is_closed
 
     def cancel(self) -> "Order":
         """Create a cancellation order. You can only cancel orders that are still open and have an id.
         The returned order looks like a regular order, but with its size set to zero.
         """
         assert self.id is not None, "Can only cancel orders with an id"
         assert self.is_open, "Can only cancel open orders"
```

### Comparing `roboquant-0.3.0/roboquant/run.py` & `roboquant-0.3.1/roboquant/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         strategy: Your strategy that you want to use. Default is None, meaning no signals will be created.
         trader: The trader you want to use. If None is specified, the `FlexTrader` will be used with its default settings
         broker: The broker you want to use. If None is specified, the `SimBroker` will be used with its default settings
         journal: Journal to use to log and/or store progress and metrics, default is None.
         timeframe: Optionally limit the run to events within this timeframe. The default is None
         capacity: The max capacity of the used event channel. Default is 10 events.
         heartbeat_timeout: Optionally, a heartbeat (is an empty event) will be generated if no other events are received
-        within the specified timeout in seconds. The default is None.
+        within the specified timeout in seconds. The default is None. This should normally only be used with live feeds since
+        the timestamp used for the heartbeat is the current time.
 
     Returns:
         The latest version of the account
     """
 
     trader = trader or FlexTrader()
     broker = broker or SimBroker()
```

### Comparing `roboquant-0.3.0/roboquant/strategies/barstrategy.py` & `roboquant-0.3.1/roboquant/strategies/tastrategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from roboquant.event import Bar
 from roboquant.signal import Signal
 from roboquant.strategies.buffer import OHLCVBuffer
 from roboquant.strategies.strategy import Strategy
 
 
-class BarStrategy(Strategy):
+class TaStrategy(Strategy):
     """Abstract base class for other strategies that helps to implement trading solutions
     based on technical indicators using bars.
 
-    Sub classes should implement the _create_signal method. This method is only invoked once
+    Subclasses should implement the _create_signal method. This method is only invoked once
     there is at least `size` history for an individual symbol.
     """
 
     def __init__(self, size: int) -> None:
         super().__init__()
         self._data: dict[str, OHLCVBuffer] = {}
         self.size = size
 
     def create_signals(self, event):
-        signals = []
+        signals: list[Signal] = []
         for item in event.items:
             if isinstance(item, Bar):
                 symbol = item.symbol
                 if symbol not in self._data:
                     self._data[symbol] = OHLCVBuffer(self.size)
                 ohlcv = self._data[symbol]
                 ohlcv.append(item.ohlcv)
```

### Comparing `roboquant-0.3.0/roboquant/strategies/buffer.py` & `roboquant-0.3.1/roboquant/strategies/buffer.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/strategies/emacrossover.py` & `roboquant-0.3.1/roboquant/strategies/emacrossover.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self._history = {}
         self.fast = 1.0 - (smoothing / (fast_period + 1))
         self.slow = 1.0 - (smoothing / (slow_period + 1))
         self.price_type = price_type
         self.min_steps = max(fast_period, slow_period)
 
     def create_signals(self, event: Event):
-        signals = []
+        signals: list[Signal] = []
         for symbol, price in event.get_prices(self.price_type).items():
 
             if symbol not in self._history:
                 self._history[symbol] = self._Calculator(self.fast, self.slow, price)
             else:
                 calculator = self._history[symbol]
                 old_rating = calculator.is_above()
```

### Comparing `roboquant-0.3.0/roboquant/strategies/multistrategy.py` & `roboquant-0.3.1/roboquant/strategies/multistrategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,9 @@
             case "avg":
                 result = []
                 g = groupby(signals, lambda x: x.symbol)
                 for symbol, v in g:
                     rating = mean(s.rating for s in v)
                     result.append(Signal(symbol, rating))
                 return result
+
+        raise ValueError("unsupported signal filter")
```

### Comparing `roboquant-0.3.0/roboquant/strategies/smacrossover.py` & `roboquant-0.3.1/roboquant/strategies/smacrossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             if prev_rating != new_rating:
                 result = Signal.buy(symbol) if new_rating else Signal.sell(symbol)
 
         self._prev_ratings[symbol] = new_rating
         return result
 
     def create_signals(self, event):
-        signals = []
+        signals: list[Signal] = []
         for (symbol, item) in event.price_items.items():
             h = self._history.get(symbol)
 
             if h is None:
                 maxlen = max(self.max_period, self.min_period)
                 h = collections.deque(maxlen=maxlen)
                 self._history[symbol] = h
```

### Comparing `roboquant-0.3.0/roboquant/strategies/strategy.py` & `roboquant-0.3.1/roboquant/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant/timeframe.py` & `roboquant-0.3.1/roboquant/timeframe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 from datetime import datetime, timedelta, timezone
 from typing import Any
 
 
 class Timeframe:
-    """A timeframe represents a period in time with a specific start- and end-datetime.
+    """A timeframe represents a period in time with a specific start- and end-datetime. Timeframes should not be mutated.
 
     Internally it stores the start and end times as Python datetime objects with the timezone set to UTC.
     """
 
     __slots__ = "start", "end", "inclusive"
 
     def __init__(self, start: datetime, end: datetime, inclusive=False):
@@ -28,48 +28,53 @@
 
     @classmethod
     def fromisoformat(cls, start: str, end: str, inclusive=False):
         s = datetime.fromisoformat(start)
         e = datetime.fromisoformat(end)
         return cls(s, e, inclusive)
 
-    @staticmethod
-    def empty():
-        return Timeframe.fromisoformat("1900-01-01T00:00:00+00:00", "1900-01-01T00:00:00+00:00", False)
+    def is_empty(self):
+        """Return true if this is an empty timeframe"""
+        return self.start == self.end and not self.inclusive
 
     @staticmethod
     def previous(inclusive=False, **kwargs):
         """Convenient method to create a historic timeframe, the kwargs arguments will be passed to the timedelta
 
-        timeframe = Timeframe.previous(days=365)
+        Usage:
+            tf = Timeframe.previous(days=365)
         """
 
         td = timedelta(**kwargs)
         end = datetime.now(timezone.utc)
         start = end - td
         return Timeframe(start, end, inclusive)
 
     @staticmethod
     def next(inclusive=False, **kwargs):
         """Convenient method to create a future timeframe, the kwargs arguments will be passed to the timedelta
 
-        timeframe = Timeframe.next(minutes=30)
+        Usage:
+            tf = Timeframe.next(minutes=30)
         """
 
         td = timedelta(**kwargs)
         start = datetime.now(timezone.utc)
         end = start + td
         return Timeframe(start, end, inclusive)
 
     def __contains__(self, time):
         if self.inclusive:
             return self.start <= time <= self.end
         return self.start <= time < self.end
 
-    def __repr__(self):
+    def __str__(self):
+        if self == EMPTY_TIMEFRAME:
+            return "EMPTY_TIMEFRAME"
+
         last_char = "]" if self.inclusive else ">"
         fmt_str = "%Y-%m-%d %H:%M:%S"
         return f"[{self.start.strftime(fmt_str)} ― {self.end.strftime(fmt_str)}{last_char}"
 
     @property
     def duration(self) -> timedelta:
         """return the duration of this timeframe expressed as timedelta"""
@@ -120,7 +125,11 @@
         return result
 
     def __eq__(self, other):
         if isinstance(other, Timeframe):
             return self.start == other.start and self.end == other.end and self.inclusive == other.inclusive
 
         return False
+
+
+EMPTY_TIMEFRAME = Timeframe.fromisoformat("1900-01-01T00:00:00+00:00", "1900-01-01T00:00:00+00:00", False)
+"""Represents an empty timeframe, one that cannot contain events"""
```

### Comparing `roboquant-0.3.0/roboquant/traders/flextrader.py` & `roboquant-0.3.1/roboquant/traders/flextrader.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,24 +40,32 @@
             return _PositionChange.ENTRY_LONG if is_buy else _PositionChange.ENTRY_SHORT
         if pos_size > 0:
             return _PositionChange.ENTRY_LONG if is_buy else _PositionChange.EXIT_LONG
 
         return _PositionChange.EXIT_SHORT if is_buy else _PositionChange.ENTRY_SHORT
 
 
-def _log_rule(rule: str, signal: Signal, symbol: str, position: Decimal):
-    if logger.isEnabledFor(logging.INFO):
-        logger.info(
-            "rating=%s type=%s symbol=%s position=%s discarded because of %s",
-            signal.rating,
-            signal.type,
-            symbol,
-            position,
-            rule,
-        )
+class _Context:
+
+    def __init__(self, signal: Signal, position: Decimal) -> None:
+        self.signal = signal
+        self.position = position
+
+    def log(self, rule: str, **kwargs):
+        if logger.isEnabledFor(logging.INFO):
+            extra = ' '.join(f"{k}={v}" for k, v in kwargs.items())
+            logger.info(
+                "Discarded signal because %s [symbol=%s rating=%s type=%s position=%s %s]",
+                rule,
+                self.signal.symbol,
+                self.signal.rating,
+                self.signal.type,
+                self.position,
+                extra,
+            )
 
 
 class FlexTrader(Trader):
     """Implementation of a Trader that has configurable rules to modify which signals are converted into orders.
     This implementation will not generate orders if there is not a price in the event for the underlying symbol.
 
     The configurable parameters include:
@@ -71,17 +79,17 @@
     - min_order_perc: the min percentage of the equity to allocate to a new order, default is 0.02 (2%)
     - shorting: allow orders that could result in a short position, default is false
     - price_type: the price type to use when determining order value, for example "CLOSE". Default is "DEFAULT"
 
     It might be sometimes challenging to understand wby a signal isn't converted into an order. The flex-trader logs
     at INFO level when certain rules have been fired.
 
-    import logging
-    logging.basicConfig(level=logging.WARNING)
-    logging.getLogger("roboquant.traders.flextrader").setLevel(logging.INFO)
+    Setting higher logging:
+        logging.basicConfig(level=logging.WARNING)
+        logging.getLogger("roboquant.traders.flextrader").setLevel(logging.INFO)
     """
 
     def __init__(
         self,
         one_order_only=True,
         size_fractions=0,
         safety_margin_perc=0.05,
@@ -123,69 +131,86 @@
         min_order_value = equity * self.min_order_perc
         max_pos_value = equity * self.max_position_perc
         available = account.buying_power - self.safety_margin_perc * equity
 
         for signal in signals:
             symbol = signal.symbol
             pos_size = account.get_position_size(symbol)
+            ctx = _Context(signal, pos_size)
+
+            change = _PositionChange.get_change(signal.is_buy, pos_size)
+
+            logger.info("available=%s signal=%s pos=%s change=%s", available, signal, pos_size, change)
 
             if self.one_order_only and account.has_open_order(symbol):
-                _log_rule("one order only", signal, symbol, pos_size)
+                ctx.log("one order only")
                 continue
 
             item = event.price_items.get(symbol)
             if item is None:
-                _log_rule("no price is available", signal, symbol, pos_size)
+                ctx.log("no price is available")
                 continue
 
             price = item.price(self.price_type)
-            change = _PositionChange.get_change(signal.is_buy, pos_size)
 
             if not self.shorting and change == _PositionChange.ENTRY_SHORT:
-                _log_rule("no shorting", signal, symbol, pos_size)
+                ctx.log("no shorting")
                 continue
 
             if change.is_exit:
                 # Closing orders don't require or use buying power
                 if not signal.is_exit:
-                    _log_rule("no exit signal", signal, symbol, pos_size)
+                    ctx.log("no exit signal")
                     continue
-                rounded_size = round(pos_size * Decimal(signal.rating), self.size_digits)
+
+                rounded_size = round(-pos_size * abs(Decimal(signal.rating)), self.size_digits)
                 if rounded_size.is_zero():
-                    _log_rule("cannot exit with order size zero", signal, symbol, pos_size)
+                    ctx.log("cannot exit with order size zero")
                     continue
                 new_orders = self._get_orders(symbol, rounded_size, item, signal, event.time)
                 orders += new_orders
             else:
+                if available < 0:
+                    ctx.log("no more available buying power")
+                    continue
+
                 if not signal.is_entry:
-                    _log_rule("no entry signal", signal, symbol, pos_size)
+                    ctx.log("no entry signal")
                     continue
 
                 if available < min_order_value:
-                    _log_rule("available buying power below minimum order value", signal, symbol, pos_size)
+                    ctx.log("available buying power below minimum order value")
                     continue
 
                 available_order_value = min(available, max_order_value, max_pos_value - abs(account.position_value(symbol)))
                 if available_order_value < min_order_value:
-                    _log_rule("calculated available order value below minimum order value", signal, symbol, pos_size)
+                    ctx.log("calculated available order value below minimum order value")
                     continue
 
                 contract_price = account.contract_value(symbol, Decimal(1), price)
                 order_size = self._get_order_size(signal.rating, contract_price, available_order_value)
 
                 if order_size.is_zero():
-                    _log_rule("calculated order size is zero", signal, symbol, pos_size)
+                    ctx.log("calculated order size is zero")
                     continue
 
                 order_value = abs(account.contract_value(symbol, order_size, price))
-                if order_value > available:
-                    _log_rule("order value above available buying power", signal, symbol, pos_size)
-                    continue
-                if order_value < min_order_value:
-                    _log_rule("order value below minimum order value", signal, symbol, pos_size)
+                if abs(order_value) > available:
+                    ctx.log(
+                        "order value above available buying power",
+                        order_value=order_value,
+                        available=available,
+                    )
+                    continue
+                if abs(order_value) < min_order_value:
+                    ctx.log(
+                        "order value below minimum order value",
+                        order_value=order_value,
+                        min_order_value=min_order_value,
+                    )
                     continue
 
                 new_orders = self._get_orders(symbol, order_size, item, signal, event.time)
                 if new_orders:
                     orders += new_orders
                     available -= order_value
```

### Comparing `roboquant-0.3.0/roboquant/traders/sizing.py` & `roboquant-0.3.1/roboquant/traders/sizing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from roboquant.event import Bar, Event
 from roboquant.feeds.yahoo import YahooFeed
 
 
 class ETR:
-    "Average True Range with a twist, it uses an exponential moving average of the true range"
+    """Average True Range with a twist, it uses an exponential moving average of the true range"""
 
     def __init__(self, period=10, smoothing=2.0):
         self.history = {}
         self.momentum = 1.0 - (smoothing / (period + 1))
 
     def add(self, event: Event):
         m = self.momentum
@@ -27,15 +27,18 @@
 
     def get_value(self, symbol) -> float | None:
         entry = self.history.get(symbol)
         if entry:
             return entry[0]
         return None
 
+    def reset(self):
+        self.history = {}
+
 
 if __name__ == "__main__":
     feed = YahooFeed("IBM", "MSFT", "TSLA")
     channel = feed.play_background()
-    e = ETR(80, 0.1)
+    e = ETR(20, 2.0)
     while evt := channel.get():
         e.add(evt)
         print(e.get_value("IBM"), e.get_value("TSLA"), e.get_value("MSFT"))
```

### Comparing `roboquant-0.3.0/roboquant/traders/trader.py` & `roboquant-0.3.1/roboquant/traders/trader.py`

 * *Files identical despite different names*

### Comparing `roboquant-0.3.0/roboquant.egg-info/PKG-INFO` & `roboquant-0.3.1/roboquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboquant
-Version: 0.3.0
+Version: 0.3.1
 Summary: A fast algo-trading platform
 Author-email: roboquant team <info@roboquant.org>
 Project-URL: Homepage, https://roboquant.org
 Project-URL: Repository, https://github.com/neurallayer/roboquant.py.git
 Project-URL: Issues, https://github.com/neurallayer/roboquant.py/issues
 Keywords: trading,investment,finance,crypto,stocks,exchange,forex
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `roboquant-0.3.0/roboquant.egg-info/SOURCES.txt` & `roboquant-0.3.1/roboquant.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 roboquant/signal.py
 roboquant/timeframe.py
 roboquant.egg-info/PKG-INFO
 roboquant.egg-info/SOURCES.txt
 roboquant.egg-info/dependency_links.txt
 roboquant.egg-info/requires.txt
 roboquant.egg-info/top_level.txt
+roboquant/alpaca/__init__.py
+roboquant/alpaca/broker.py
+roboquant/alpaca/feed.py
 roboquant/brokers/__init__.py
-roboquant/brokers/alpacabroker.py
 roboquant/brokers/broker.py
 roboquant/brokers/ibkr.py
 roboquant/brokers/simbroker.py
 roboquant/feeds/__init__.py
 roboquant/feeds/aggregate.py
-roboquant/feeds/alpacafeed.py
+roboquant/feeds/avrofeed.py
+roboquant/feeds/collect.py
 roboquant/feeds/csvfeed.py
 roboquant/feeds/eventchannel.py
 roboquant/feeds/feed.py
 roboquant/feeds/feedutil.py
 roboquant/feeds/historic.py
 roboquant/feeds/live.py
 roboquant/feeds/randomwalk.py
@@ -45,17 +48,17 @@
 roboquant/journals/runmetric.py
 roboquant/journals/tensorboardjournal.py
 roboquant/ml/__init__.py
 roboquant/ml/envs.py
 roboquant/ml/features.py
 roboquant/ml/strategies.py
 roboquant/strategies/__init__.py
-roboquant/strategies/barstrategy.py
 roboquant/strategies/buffer.py
 roboquant/strategies/emacrossover.py
 roboquant/strategies/multistrategy.py
 roboquant/strategies/smacrossover.py
 roboquant/strategies/strategy.py
+roboquant/strategies/tastrategy.py
 roboquant/traders/__init__.py
 roboquant/traders/flextrader.py
 roboquant/traders/sizing.py
 roboquant/traders/trader.py
```

