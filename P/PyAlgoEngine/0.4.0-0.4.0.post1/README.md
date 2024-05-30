# Comparing `tmp/pyalgoengine-0.4.0.tar.gz` & `tmp/pyalgoengine-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalgoengine-0.4.0.tar", last modified: Wed May 29 07:24:17 2024, max compression
+gzip compressed data, was "pyalgoengine-0.4.0.post1.tar", last modified: Wed May 29 07:55:31 2024, max compression
```

## Comparing `pyalgoengine-0.4.0.tar` & `pyalgoengine-0.4.0.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.697980 pyalgoengine-0.4.0/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      769 2024-05-29 07:24:17.683160 pyalgoengine-0.4.0/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.679160 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      769 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      747 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       77 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-29 07:24:17.000000 pyalgoengine-0.4.0/PyAlgoEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0/README.md
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.373379 pyalgoengine-0.4.0/algo_engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1936 2024-05-29 07:16:50.000000 pyalgoengine-0.4.0/algo_engine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.418403 pyalgoengine-0.4.0/algo_engine/back_test/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      232 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1821 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/back_test/__main__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9216 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/replay.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14126 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/back_test/sim_match.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.535651 pyalgoengine-0.4.0/algo_engine/engine/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      672 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31180 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/engine/algo_engine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1354 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/event_engine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    11697 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0/algo_engine/engine/market_engine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    69005 2024-05-29 06:58:50.000000 pyalgoengine-0.4.0/algo_engine/engine/trade_engine.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.579651 pyalgoengine-0.4.0/algo_engine/monitor/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      449 2024-05-28 11:24:54.000000 pyalgoengine-0.4.0/algo_engine/monitor/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     8940 2024-05-28 10:54:06.000000 pyalgoengine-0.4.0/algo_engine/monitor/advanced_data_interface.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.624159 pyalgoengine-0.4.0/algo_engine/profile/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1900 2024-05-29 07:03:58.000000 pyalgoengine-0.4.0/algo_engine/profile/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7052 2024-05-28 11:28:56.000000 pyalgoengine-0.4.0/algo_engine/profile/cn.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:24:17.668160 pyalgoengine-0.4.0/algo_engine/strategie/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1619 2024-05-29 07:16:50.000000 pyalgoengine-0.4.0/algo_engine/strategie/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    15413 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/algo_engine/strategie/strategy_engine.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-29 07:24:17.702980 pyalgoengine-0.4.0/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1649 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.649186 pyalgoengine-0.4.0.post1/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0.post1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      775 2024-05-29 07:55:31.646187 pyalgoengine-0.4.0.post1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.642928 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      775 2024-05-29 07:55:31.000000 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      747 2024-05-29 07:55:31.000000 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-29 07:55:31.000000 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       77 2024-05-29 07:55:31.000000 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-29 07:55:31.000000 pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       42 2024-05-15 04:37:41.000000 pyalgoengine-0.4.0.post1/README.md
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.407962 pyalgoengine-0.4.0.post1/algo_engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1942 2024-05-29 07:44:44.000000 pyalgoengine-0.4.0.post1/algo_engine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.459622 pyalgoengine-0.4.0.post1/algo_engine/back_test/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      232 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/back_test/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1821 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0.post1/algo_engine/back_test/__main__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9216 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/back_test/replay.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    14126 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/back_test/sim_match.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.544162 pyalgoengine-0.4.0.post1/algo_engine/engine/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      672 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/engine/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    31182 2024-05-29 07:47:20.000000 pyalgoengine-0.4.0.post1/algo_engine/engine/algo_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1354 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/engine/event_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    11697 2024-05-29 06:54:26.000000 pyalgoengine-0.4.0.post1/algo_engine/engine/market_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    69005 2024-05-29 06:58:50.000000 pyalgoengine-0.4.0.post1/algo_engine/engine/trade_engine.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.578227 pyalgoengine-0.4.0.post1/algo_engine/monitor/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      449 2024-05-28 11:24:54.000000 pyalgoengine-0.4.0.post1/algo_engine/monitor/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     8940 2024-05-28 10:54:06.000000 pyalgoengine-0.4.0.post1/algo_engine/monitor/advanced_data_interface.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.592162 pyalgoengine-0.4.0.post1/algo_engine/profile/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1900 2024-05-29 07:03:58.000000 pyalgoengine-0.4.0.post1/algo_engine/profile/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7070 2024-05-29 07:44:07.000000 pyalgoengine-0.4.0.post1/algo_engine/profile/cn.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-29 07:55:31.634228 pyalgoengine-0.4.0.post1/algo_engine/strategie/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1620 2024-05-29 07:49:01.000000 pyalgoengine-0.4.0.post1/algo_engine/strategie/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    15413 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0.post1/algo_engine/strategie/strategy_engine.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-29 07:55:31.649186 pyalgoengine-0.4.0.post1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1649 2024-05-29 07:23:17.000000 pyalgoengine-0.4.0.post1/setup.py
```

### Comparing `pyalgoengine-0.4.0/LICENSE` & `pyalgoengine-0.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/PKG-INFO` & `pyalgoengine-0.4.0.post1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.4.0
+Version: 0.4.0.post1
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyalgoengine-0.4.0/PyAlgoEngine.egg-info/PKG-INFO` & `pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAlgoEngine
-Version: 0.4.0
+Version: 0.4.0.post1
 Summary: Basic algo engine
 Home-page: https://github.com/BolunHan/PyAlgoEngine
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pyalgoengine-0.4.0/PyAlgoEngine.egg-info/SOURCES.txt` & `pyalgoengine-0.4.0.post1/PyAlgoEngine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/__init__.py` & `pyalgoengine-0.4.0.post1/algo_engine/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.0.post1"
 
 import logging
 import os
 import sys
 import time
 import traceback
```

### Comparing `pyalgoengine-0.4.0/algo_engine/back_test/__main__.py` & `pyalgoengine-0.4.0.post1/algo_engine/back_test/__main__.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/back_test/replay.py` & `pyalgoengine-0.4.0.post1/algo_engine/back_test/replay.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/back_test/sim_match.py` & `pyalgoengine-0.4.0.post1/algo_engine/back_test/sim_match.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/engine/__init__.py` & `pyalgoengine-0.4.0.post1/algo_engine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/engine/algo_engine.py` & `pyalgoengine-0.4.0.post1/algo_engine/engine/algo_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     rejected = 'rejected'  # internal / external rejected
     error = 'error'  # internal / external error
 
 
 class AlgoTemplate(object, metaclass=abc.ABCMeta):
     Status = AlgoStatus
 
-    def __init__(self, dma: DirectMarketAccess, ticker: str, target_volume: float, side: TransactionSide, **kwargs):
+    def __init__(self, dma: 'DirectMarketAccess', ticker: str, target_volume: float, side: TransactionSide, **kwargs):
         """ Template for trading algorithm
         an abstract class to create a trading algorithm
 
         :param dma: direct market access
         :param ticker: the given symbol of the underlying to trade
         :param target_volume: the given volume to trade
         :param side: the given TransactionSide
```

### Comparing `pyalgoengine-0.4.0/algo_engine/engine/event_engine.py` & `pyalgoengine-0.4.0.post1/algo_engine/engine/event_engine.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/engine/market_engine.py` & `pyalgoengine-0.4.0.post1/algo_engine/engine/market_engine.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/engine/trade_engine.py` & `pyalgoengine-0.4.0.post1/algo_engine/engine/trade_engine.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/monitor/advanced_data_interface.py` & `pyalgoengine-0.4.0.post1/algo_engine/monitor/advanced_data_interface.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/profile/__init__.py` & `pyalgoengine-0.4.0.post1/algo_engine/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/algo_engine/profile/cn.py` & `pyalgoengine-0.4.0.post1/algo_engine/profile/cn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import functools
 
 from . import Profile
 
 
 class CN_Profile(Profile):
     def __init__(self):
```

### Comparing `pyalgoengine-0.4.0/algo_engine/strategie/__init__.py` & `pyalgoengine-0.4.0.post1/algo_engine/strategie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from threading import Lock
 
 from PyQuantKit import TradeInstruction
 
-from .strategy_engine import StrategyEngine
 from .. import LOGGER
 from ..engine import EVENT_ENGINE, TOPIC, MDS, MarketDataService, Balance, Inventory, DirectMarketAccess, RiskProfile, PositionManagementService
 
 LOGGER = LOGGER.getChild('Strategies')
 
+from .strategy_engine import StrategyEngine
+
 
 class EventDMA(DirectMarketAccess):
     def __init__(self, mds: MarketDataService, risk_profile: RiskProfile, event_engine=None, cool_down: float = None):
         self.event_engine = EVENT_ENGINE if event_engine is None else event_engine
         super().__init__(mds=mds, risk_profile=risk_profile, cool_down=cool_down)
 
     def _launch_order_handler(self, order: TradeInstruction, **kwargs):
```

### Comparing `pyalgoengine-0.4.0/algo_engine/strategie/strategy_engine.py` & `pyalgoengine-0.4.0.post1/algo_engine/strategie/strategy_engine.py`

 * *Files identical despite different names*

### Comparing `pyalgoengine-0.4.0/setup.py` & `pyalgoengine-0.4.0.post1/setup.py`

 * *Files identical despite different names*

