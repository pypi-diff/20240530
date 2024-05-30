# Comparing `tmp/pyquantkit-0.3.0.tar.gz` & `tmp/pyquantkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquantkit-0.3.0.tar", last modified: Tue May 28 02:25:31 2024, max compression
+gzip compressed data, was "pyquantkit-0.3.1.tar", last modified: Thu May 30 04:10:49 2024, max compression
```

## Comparing `pyquantkit-0.3.0.tar` & `pyquantkit-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.216126 pyquantkit-0.3.0/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-28 02:25:31.213126 pyquantkit-0.3.0/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.109828 pyquantkit-0.3.0/PyQuantKit/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    68097 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/PyQuantKit/MarketUtils_old.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    19556 2024-05-27 06:25:36.000000 pyquantkit-0.3.0/PyQuantKit/TradeUtils_old.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7923 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/PyQuantKit/_FinanceDecimal.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3207 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    35847 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/console_utils.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    51864 2024-05-27 06:25:36.000000 pyquantkit-0.3.0/PyQuantKit/market_utils.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    16197 2024-05-27 09:21:24.000000 pyquantkit-0.3.0/PyQuantKit/technical_analysis.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    22613 2024-05-27 09:56:50.000000 pyquantkit-0.3.0/PyQuantKit/trade_utils.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 02:25:31.191125 pyquantkit-0.3.0/PyQuantKit.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      421 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/requires.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2024-05-28 02:25:30.000000 pyquantkit-0.3.0/PyQuantKit.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       53 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-28 02:25:31.217126 pyquantkit-0.3.0/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1491 2024-05-27 03:33:46.000000 pyquantkit-0.3.0/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-30 04:10:49.387204 pyquantkit-0.3.1/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-27 03:33:46.000000 pyquantkit-0.3.1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-30 04:10:49.383203 pyquantkit-0.3.1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-30 04:10:49.253163 pyquantkit-0.3.1/PyQuantKit/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     7923 2024-05-27 03:33:46.000000 pyquantkit-0.3.1/PyQuantKit/_FinanceDecimal.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3207 2024-05-30 04:10:27.000000 pyquantkit-0.3.1/PyQuantKit/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    35847 2024-05-27 09:21:24.000000 pyquantkit-0.3.1/PyQuantKit/console_utils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    51864 2024-05-27 06:25:36.000000 pyquantkit-0.3.1/PyQuantKit/market_utils.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    16197 2024-05-27 09:21:24.000000 pyquantkit-0.3.1/PyQuantKit/technical_analysis.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    22620 2024-05-30 03:49:22.000000 pyquantkit-0.3.1/PyQuantKit/trade_utils.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-30 04:10:49.379203 pyquantkit-0.3.1/PyQuantKit.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      604 2024-05-30 04:10:49.000000 pyquantkit-0.3.1/PyQuantKit.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      362 2024-05-30 04:10:49.000000 pyquantkit-0.3.1/PyQuantKit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-30 04:10:49.000000 pyquantkit-0.3.1/PyQuantKit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       13 2024-05-30 04:10:49.000000 pyquantkit-0.3.1/PyQuantKit.egg-info/requires.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       11 2024-05-30 04:10:49.000000 pyquantkit-0.3.1/PyQuantKit.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       53 2024-05-27 03:33:46.000000 pyquantkit-0.3.1/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       38 2024-05-30 04:10:49.388203 pyquantkit-0.3.1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1491 2024-05-27 03:33:46.000000 pyquantkit-0.3.1/setup.py
```

### Comparing `pyquantkit-0.3.0/LICENSE` & `pyquantkit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquantkit-0.3.0/PKG-INFO` & `pyquantkit-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyquantkit-0.3.0/PyQuantKit/MarketUtils_old.py` & `pyquantkit-0.3.1/PyQuantKit/market_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
+from multiprocessing import RawValue, RawArray
+from ctypes import c_ulong, c_double, c_wchar, c_int, c_longlong
 import abc
-import bisect
 import datetime
 import enum
 import json
 import math
 import re
 import warnings
-from collections import defaultdict
-from typing import overload, Iterable
+from typing import overload
 
 import numpy as np
-import pandas as pd
 
-from . import LOGGER
+from . import LOGGER, TIME_ZONE
 
 LOGGER = LOGGER.getChild('MarketUtils')
-__all__ = ['BarData', 'MarketData', 'OrderBook', 'TickData', 'TransactionData', 'TradeData', 'TransactionSide', 'TradeSide', 'get_data_attr', 'convert_to_bar']
+__all__ = ['TransactionSide',
+           'MarketData', 'OrderBook', 'BarData', 'TickData', 'TransactionData', 'TradeData',
+           'OrderBookBuffer', 'BarDataBuffer', 'TickDataBuffer', 'TransactionDataBuffer']
 
 
 class TransactionSide(enum.Enum):
     ShortOrder = AskOrder = Offer_to_Short = -3
     ShortOpen = Sell_to_Short = -2
     ShortFilled = LongClose = Sell_to_Unwind = ask = -1
     UNKNOWN = CANCEL = 0
@@ -172,127 +173,122 @@
         elif self.value == self.Offer_to_Short.value or self.value == self.Bid_to_Long.value:
             LOGGER.warning(f'Requesting offset of {self.name} is not supported, returns {self.side_name}')
             return self.side_name
         else:
             return 'Unknown'
 
 
-TradeSide = TransactionSide
+class MarketData(dict, metaclass=abc.ABCMeta):
+    def __init__(self, ticker: str, timestamp: float, **kwargs):
+        super().__init__(ticker=ticker, timestamp=timestamp)
 
-
-class MarketData(object):
-    """
-    Abstract parent class of BarData, TickData, TradeData and OrderBook
-    """
-
-    def __init__(self, ticker: str, timestamp: float):
-        self.ticker = ticker
-        self.timestamp = timestamp
-
-    def __reduce__(self):
-        return self.__class__.from_json, (self.to_json(),)
-
-    def __hash__(self):
-        return id(self)
+        if kwargs:
+            self['additional'] = dict(kwargs)
 
     def __copy__(self):
-        return self.__class__.from_json(self.to_json(fmt='dict'))
+        return self.__class__.__init__(**self)
 
     def copy(self):
         return self.__copy__()
 
-    @property
-    @abc.abstractmethod
-    def market_time(self) -> datetime.datetime | datetime.date | float | int:
-        ...
+    def to_json(self, fmt='str', **kwargs) -> str | dict:
+        data_dict = dict(
+            dtype=self.__class__.__name__,
+            **self
+        )
 
-    @property
-    @abc.abstractmethod
-    def market_price(self) -> float:
-        ...
+        if 'additional' in data_dict:
+            additional = data_dict.pop('additional')
+            data_dict.update(additional)
 
-    @abc.abstractmethod
-    def to_json(self, **kwargs) -> str:
-        ...
+        if fmt == 'dict':
+            return data_dict
+        elif fmt == 'str':
+            return json.dumps(data_dict, **kwargs)
+        else:
+            raise ValueError(f'Invalid format {fmt}, except "dict" or "str".')
 
     @classmethod
     def from_json(cls, json_message: str | bytes | bytearray | dict) -> MarketData:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
-        dtype = json_dict.get('dtype', None)
+        dtype = json_dict.pop('dtype', None)
         if dtype == 'BarData':
             return BarData.from_json(json_dict)
         elif dtype == 'TickData':
             return TickData.from_json(json_dict)
+        elif dtype == 'TransactionData':
+            return TransactionData.from_json(json_dict)
         elif dtype == 'TradeData':
             return TradeData.from_json(json_dict)
         elif dtype == 'OrderBook':
             return OrderBook.from_json(json_dict)
         else:
             raise TypeError(f'Invalid dtype {dtype}')
 
-    @property
-    def topic(self):
-        return f'{self.ticker}.{self.__class__.__name__}'
+    @abc.abstractmethod
+    def to_list(self) -> list[float | int | str | bool]:
+        ...
 
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> MarketData:
+        dtype = data_list[0]
 
-class OrderBook(MarketData):
-    class OrderBookEntry(object):
+        if dtype == 'BarData':
+            return BarData.from_list(data_list)
+        elif dtype == 'TickData':
+            return TickData.from_list(data_list)
+        elif dtype == 'TransactionData':
+            return TransactionData.from_list(data_list)
+        elif dtype == 'TradeData':
+            return TradeData.from_list(data_list)
+        elif dtype == 'OrderBook':
+            return OrderBook.from_list(data_list)
+        else:
+            raise TypeError(f'Invalid dtype {dtype}')
 
-        """
-        A OrderBook log Entry
-        :param price: listed price
-        :param volume: total listed volume at given price
-        :param side: bid or ask
-        """
+    @property
+    def ticker(self):
+        return self['ticker']
 
-        def __init__(
-                self,
-                price: float = 'nan',
-                volume: float = 0.,
-                side: TransactionSide | str | int = 0
-        ):
-            self.price = float(price)
-            self.side = TransactionSide(side)
-            self.volume = float(volume)
+    @property
+    def timestamp(self):
+        return self['timestamp']
 
-        @property
-        def side_name(self) -> str:
-            if self.side.order_sign > 0:
-                return 'bid'
-            else:
-                return 'ask'
+    @property
+    def additional(self):
+        if 'additional' not in self:
+            self['additional'] = {}
+        return self['additional']
 
-        def __lt__(self, other):
-            if self.side.order_sign > 0:  # bid book
-                if isinstance(other, self.__class__):
-                    return self.price > other.price
-                else:
-                    return self.price > other
-            else:  # ask book
-                if isinstance(other, self.__class__):
-                    return self.price < other.price
-                else:
-                    return self.price < other
+    @property
+    def topic(self) -> str:
+        return f'{self.ticker}.{self.__class__.__name__}'
 
-        def __repr__(self):
-            return f'<OrderBookEntry.{self.side_name.capitalize()}>({self.price:,.2f}: {self.volume:,.2f})'
+    @property
+    def market_time(self) -> datetime.datetime | datetime.date:
+        return datetime.datetime.fromtimestamp(self.timestamp, tz=TIME_ZONE)
 
-        def __bool__(self):
-            return self.volume > 0
+    @property
+    @abc.abstractmethod
+    def market_price(self) -> float:
+        ...
 
-    class Book(object):
 
-        def __init__(self, side):
-            self.side = TransactionSide(side)
-            self._book: list[OrderBook.OrderBookEntry] = []
-            self._dict: dict[float, OrderBook.OrderBookEntry] = {}
+class OrderBook(MarketData):
+    class Book(object):
+        def __init__(self, side: int):
+            self.side: int = side
+            # store the entry in order of (price, volume, order, etc...)
+            self._book: list[tuple[float, float, ...]] = []
+            self._dict: dict[float, tuple[float, float, ...]] = {}
+            self.sorted = False
 
         def __iter__(self):
             self.sort()
             return sorted(self._book).__iter__()
 
         def __getitem__(self, item):
             if isinstance(item, int) and item not in self._dict:
@@ -305,74 +301,70 @@
         def __contains__(self, price: float):
             return self._dict.__contains__(price)
 
         def __len__(self):
             return self._book.__len__()
 
         def __repr__(self):
-            return f'<OrderBook.Book.{"Bid" if self.side > 0 else "Ask"}>[{", ".join([f"({entry.price:,.2f}: {entry.volume:,.2f})" for entry in self._book])}]'
+            return f'<OrderBook.Book.{"Bid" if self.side > 0 else "Ask"}>'
 
         def __bool__(self):
-            return bool(self._book) and all(self._book)
+            return bool(self._book)
 
         def __sub__(self, other: OrderBook.Book) -> dict[float, float]:
             if not isinstance(other, self.__class__):
-                raise TypeError(f'Expect type {self.__class__}, got {type(other)}')
+                raise TypeError(f'Expect type {self.__class__.__name__}, got {type(other)}')
 
-            if self.side.order_sign != other.side.order_sign:
+            if self.side != other.side:
                 raise ValueError(f'Expect side {self.side}, got {other.side}')
 
             diff = {}
 
             # bid book
             if (not self._dict) or (not other._dict):
                 pass
-            elif self.side.order_sign > 0:
+            elif self.side > 0:
                 limit_0 = min(self._dict)
                 limit_1 = min(other._dict)
                 limit = max(limit_0, limit_1)
                 contain_limit = True if limit_0 == limit_1 else False
 
-                for _ in self:
-                    price = _.price
-                    volume = _.volume
+                for entry in self._book:
+                    price, volume, *_ = entry
 
                     if price > limit or (price >= limit and contain_limit):
                         diff[price] = volume
 
-                for _ in other:
-                    price = _.price
-                    volume = _.volume
+                for entry in other._book:
+                    price, volume, *_ = entry
 
                     if price > limit or (price >= limit and contain_limit):
                         diff[price] = diff.get(price, 0.) - volume
             # ask book
             else:
                 limit_0 = max(self._dict)
                 limit_1 = max(other._dict)
                 limit = min(limit_0, limit_1)
                 contain_limit = True if limit_0 == limit_1 else False
 
-                for _ in self:
-                    price = _.price
-                    volume = _.volume
+                for entry in self._book:
+                    price, volume, *_ = entry
 
                     if price < limit or (price <= limit and contain_limit):
                         diff[price] = volume
 
-                for _ in other:
-                    price = _.price
-                    volume = _.volume
+                for entry in other._book:
+                    price, volume, *_ = entry
 
                     if price < limit or (price <= limit and contain_limit):
                         diff[price] = diff.get(price, 0.) - volume
 
             return diff
 
-        def get(self, item=None, **kwargs) -> OrderBook.OrderBookEntry | None:
+        def get(self, item=None, **kwargs) -> tuple[float, float, ...] | None:
             if item is None:
                 price = kwargs.pop('price', None)
                 level = kwargs.pop('level', None)
             else:
                 if isinstance(item, int):
                     price = None
                     level = item
@@ -393,14 +385,29 @@
                 try:
                     return self.at_price(price=price)
                 except KeyError:
                     return None
             else:
                 raise ValueError('Must NOT assign both price or level in kwargs')
 
+        def pop(self, price: float):
+            entry = self._dict.pop(price, None)
+            if entry is not None:
+                self._book.remove(entry)
+            else:
+                raise KeyError(f'Price {price} not exist in order book')
+            return entry
+
+        def remove(self, entry: OrderBook.OrderBookEntry):
+            try:
+                self._book.remove(entry)
+                self._dict.pop(entry.price)
+            except ValueError:
+                raise ValueError(f'Entry {entry} not exist in order book')
+
         def at_price(self, price: float):
             """
             get OrderBook.Book.Entry with specific price
             :param price: the given price
             :return: the logged OrderBook.Book.Entry
             """
             if price in self._dict:
@@ -412,582 +419,447 @@
             """
             get OrderBook.Book.Entry with level num
             :param level: the given level
             :return: the logged OrderBook.Book.Entry
             """
             return self._book.__getitem__(level)
 
-        def add(self, price: float, volume: float, **kwargs):
-            self.add_entry(price=price, volume=volume)
-
-        def add_entry(self, price: float, volume: float):
-            entry = OrderBook.OrderBookEntry(price=price, volume=volume, side=self.side)
-            bisect.insort(self._book, entry)
-            if not math.isnan(price):
-                self._dict[price] = entry
-            return entry
-
-        def update_entry(self, price: float, volume: float):
+        def update(self, price: float, volume: float, order: int = None):
             if price in self._dict:
                 if volume == 0:
                     self.pop(price=price)
                 elif volume < 0:
                     LOGGER.warning(f'Invalid volume {volume}, expect a positive float.')
                     self.pop(price=price)
                 else:
                     entry = self._dict[price]
                     entry.volume = volume
             else:
-                self.add_entry(price=price, volume=volume)
-
-        def append(self, entry: OrderBook.OrderBookEntry) -> None:
-            if not isinstance(entry, OrderBook.OrderBookEntry):
-                raise TypeError(f'Can only append [Entry] item to [Book], but received [{type(entry)}]')
+                self.add(price=price, volume=volume, order=order)
 
+        def add(self, price: float, volume: float, order: int = None):
+            entry = (price, volume, order if order else 0)
+            self._dict[price] = entry
             self._book.append(entry)
 
-            if not math.isnan(entry.price):
-                self._dict[entry.price] = entry
-
-        def pop(self, price: float):
-            entry = self._dict.pop(price, None)
-            if entry is not None:
-                self._book.remove(entry)
-            else:
-                raise KeyError(f'Price {price} not exist in order book')
-            return entry
-
-        def remove(self, entry: OrderBook.OrderBookEntry):
-            try:
-                self._book.remove(entry)
-                self._dict.pop(entry.price)
-            except ValueError:
-                raise ValueError(f'Entry {entry} not exist in order book')
-
-        def loc(self, prior: float = None, posterior: float = None):
-            """
-            loc transactions prior or posterior to given price. NOT COUNTING EQUAL!
-            :param prior: the given price
-            :param posterior: the given price
-            :return: the summed transaction volume
-            """
+        def loc_volume(self, p0: float, p1: float):
             volume = 0.
-            if prior is None and posterior is None:
-                raise ValueError('Must assign either prior or posterior in kwargs')
-            elif posterior is None:
-                for entry in self._book:
-                    if entry.price > prior and self.side.order_sign > 0:
-                        volume += entry.volume
-                    elif entry.price < prior and self.side.order_sign < 0:
-                        volume += entry.volume
-            elif prior is None:
-                for entry in self._book:
-                    if entry.price < posterior and self.side.order_sign > 0:
-                        volume += entry.volume
-                    elif entry.price > posterior and self.side.order_sign < 0:
-                        volume += entry.volume
-            else:
-                for entry in self._book:
-                    if posterior > entry.price > prior and self.side.order_sign > 0:
-                        volume += entry.volume
-                    elif posterior < entry.price < prior and self.side.order_sign < 0:
-                        volume += entry.volume
-
-            return volume
-
-        def refresh(self):
-            _dict = {}
-            _book = []
+            p_min = min(p0, p1)
+            p_max = max(p0, p1)
 
             for entry in self._book:
-                if entry.volume == 0:
-                    pass
-                elif math.isnan(entry.price):
-                    _book.append(entry)
-                else:
-                    _book.append(entry)
-                    _dict[entry.price] = entry
+                price, volume, *_ = entry
+                if p_min < price < p_max:
+                    volume += volume
 
-            self._book = _book
-            self._dict = _dict
+            return volume
 
         def sort(self):
-            if self.side.order_sign > 0:
-                self._book.sort(reverse=True, key=lambda x: x.price)
+            if self.side > 0:  # bid
+                self._book.sort(reverse=True, key=lambda x: x[0])
             else:
-                self._book.sort(key=lambda x: x.price)
+                self._book.sort(key=lambda x: x[0])
+            self.sorted = True
 
         @property
         def price(self):
-            self.sort()
-            return [entry.price for entry in self._book]
+            if not self.sorted:
+                self.sort()
+
+            return [entry[0] for entry in self._book]
 
         @property
         def volume(self):
-            self.sort()
-            return [entry.volume for entry in self._book]
-
-    def __init__(
-            self, *,
-            ticker: str,
-            market_time: datetime.datetime = None,
-            timestamp: float = None,
-            bid: Book = None,
-            ask: Book = None,
-            **kwargs
-    ):
-        """
-        MarketData object to store the snapshot of order book at given time
-        :param ticker: the given ticker (symbol) of the trading asset
-        :param market_time: the datetime of the snapshot
-        :param bid: optional, a OrderBook.Book object store the order books at bid side. Recommend to input data with OrderBook.update() or OrderBook.Book.add() method
-        :param ask: optional, a OrderBook.Book object store the order books at ask side
-        :param kwargs: additional data send to OrderBook.update() method
-        """
-        super().__init__(
-            ticker=ticker,
-            timestamp=market_time.timestamp() if timestamp is None else timestamp
-        )
-
-        if bid is None:
-            self.bid = self.Book(side=TransactionSide.BidOrder)
-        elif isinstance(bid, self.__class__.Book):
-            if bid.side == TransactionSide.BidOrder:
-                self.bid = bid
-            else:
-                raise ValueError(f'Invalid OrderBook.bid.side, expect {TransactionSide.bid}, got {bid.side}')
-        else:
-            raise TypeError(f'Invalid OrderBook.bid, expect type {OrderBook.Book}, got {type(bid)}')
+            if not self.sorted:
+                self.sort()
 
-        if ask is None:
-            self.ask = self.Book(side=TransactionSide.AskOrder)
-        elif isinstance(ask, self.__class__.Book):
-            if ask.side == TransactionSide.AskOrder:
-                self.ask = ask
-            else:
-                raise ValueError(f'Invalid OrderBook.ask.side, expect {TransactionSide.ask}, got {ask.side}')
-        else:
-            raise TypeError(f'Invalid OrderBook.ask, expect type {OrderBook.Book}, got {type(ask)}')
+            return [entry[1] for entry in self._book]
 
-        self.additional = {}
-        self.update(**kwargs)
-
-    def __call__(self, **kwargs):
-        self.update(**kwargs)
+    def __init__(self, *, ticker: str, timestamp: float, bid: list[list[float | int]] = None, ask: list[list[float | int]] = None, **kwargs):
+        super().__init__(ticker=ticker, timestamp=timestamp)
+        self.update(
+            bid=[] if bid is None else bid,
+            ask=[] if ask is None else ask
+        )
+        self.parse(**kwargs)
 
     def __getattr__(self, item: str):
         if re.match('^((bid_)|(ask_))((price_)|(volume_))[0-9]+$', item):
             side = item.split('_')[0]
             key = item.split('_')[1]
             level = int(item.split('_')[2])
             book: 'OrderBook.Book' = self.__getattribute__(f'{side}')
             if 0 < level <= len(book):
                 return book[level].__getattribute__(key)
             else:
                 raise AttributeError(f'query level [{level}] exceed max level [{len(book)}]')
         else:
             raise AttributeError(f'{item} not found in {self.__class__}')
 
-    def __getitem__(self, item):
-        return self.__getattr__(item=item)
-
     def __setattr__(self, key, value):
         if re.match('^((bid_)|(ask_))((price_)|(volume_))[0-9]+$', key):
             self.update({key: value})
         else:
             super().__setattr__(key, value)
 
     def __repr__(self):
-        return f'<OrderBook>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker} {{Bid: [{", ".join([f"({entry.price:,.2f}: {entry.volume:,.2f})" for entry in self.bid])}], Ask: [{", ".join([f"({entry.price:,.2f}: {entry.volume:,.2f})" for entry in self.ask])}]}})'
+        return f'<OrderBook>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker}, bid={self.best_bid_price}, ask={self.best_ask_price})'
 
     def __str__(self):
         return f'<OrderBook>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker} {{Bid: {self.best_bid_price, self.best_bid_volume}, Ask: {self.best_ask_price, self.best_ask_volume}, Level: {self.max_level}}})'
 
     def __bool__(self):
         return bool(self.bid) and bool(self.ask)
 
-    def __sub__(self, other: OrderBook):
-        if not isinstance(other, self.__class__):
-            raise TypeError(f'Expect type {self.__class__}, got {type(other)}')
-
-        if self.ticker != other.ticker:
-            raise ValueError(f'Expect ticker {self.ticker}, got {other.ticker}')
-
-        if self.timestamp < other.timestamp:
-            LOGGER.warning(f'Expect subtracted by newer order book, timestamp should >= {self.timestamp}, got {other.timestamp}')
-
-        bid_diff = self.bid - other.bid
-        ask_diff = self.ask - other.ask
-
-        _ = OrderBookDiff(
-            ticker=self.ticker,
-            timestamp=other.timestamp,
-            bid_diff=bid_diff,
-            ask_diff=ask_diff
-        )
+    @classmethod
+    def _parse_entry_name(cls, name: str, validate: bool = False) -> tuple[str, str, int]:
+        if validate:
+            if not re.match('^((bid_)|(ask_))((price_)|(volume_)|(order_))[0-9]+$', name):
+                raise ValueError(f'Can not parse kwargs {name}.')
 
-        return _
+        side, key, level = name.split('_')
+        level = int(level)
+
+        return side, key, level
 
     @overload
-    def update(
-            self,
-            data: dict[str, float] = None,
-            /,
-            bid_price_1: float = math.nan,
-            bid_volume_1: float = math.nan,
-            ask_price_1: float = math.nan,
-            ask_volume_1: float = math.nan,
-            **kwargs: float
-    ):
+    def parse(self, data: dict[str, float] = None, /, bid_price_1: float = math.nan, bid_volume_1: float = math.nan, ask_price_1: float = math.nan, ask_volume_1: float = math.nan, **kwargs: float):
         ...
 
-    def update(self, data: dict[str, float] = None, **kwargs):
+    def parse(self, data: dict[str, float] = None, validate: bool = False, **kwargs):
         if not data:
             data = {}
 
         data.update(kwargs)
 
-        if not data:
-            LOGGER.debug(f'{self.__class__} has nothing to update, but still will purge the cache!')
+        for name, value in data.items():
+            split_str = name.split('_')
 
-        for name in data:
-            if re.match('^((bid_)|(ask_))((price_)|(volume_))[0-9]+$', name):
-                # validate data
-                side = name.split('_')[0]
-                key = name.split('_')[1]
-                level = int(name.split('_')[2])
-                value = data[name]
-                book: OrderBook.Book = self.__getattribute__(f'{side}')
+            if validate:
+                if len(split_str) != 3:
+                    self.additional[name] = value
 
-                if level <= 0:
-                    raise ValueError(f'Level of name [{name}] must be greater than zero!')
+                side, key, level = name.split('_')
 
-                while level > len(book):
-                    book.append(self.OrderBookEntry(price=np.nan))
+                if not (side == 'bid' or side == 'ask'):
+                    self.additional[name] = value
 
-                book.at_level(level - 1).__setattr__(key, value)
-            else:
-                self.additional[name] = data[name]
-                LOGGER.warning(f'invalid name {name}, but still will store the data')
+                if not (key == 'price' or key == 'volume' or key == 'order'):
+                    self.additional[name] = value
 
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'timestamp': self.timestamp,
-            'bid': [(entry.price, entry.volume) for entry in self.bid],
-            'ask': [(entry.price, entry.volume) for entry in self.ask],
-        }
+                if level.isnumeric():
+                    level = int(level)
+                else:
+                    self.additional[name] = value
+            else:
+                side, key, level = name.split('_')
+                level = int(level)
 
-        if self.additional:
-            data_dict['additional'] = self.additional
+            book: list = self[side]
 
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+            if level <= 0:
+                raise ValueError(f'Level of name [{name}] must be greater than zero!')
 
-    def get_book(self, side: TransactionSide, opposite=False) -> Book:
-        """
-        get corresponding order book. Buy -> bid book | Sell -> ask book
-        :param side: the given trade side
-        :param opposite: to return opposite book
-        :return: a book
-        """
-        side_sign = side.sign
+            if key == 'price':
+                entry_idx = 0
+            elif key == 'volume':
+                entry_idx = 1
+            elif key == 'order':
+                entry_idx = 2
+            else:
+                raise ValueError(f'Can not parse kwargs {name}.')
 
-        if opposite:
-            side_sign = -side_sign
+            while level > len(book):
+                book.append([math.nan, 0, 0])
 
-        if side_sign > 0:
-            return self.bid
-        elif side_sign < 0:
-            return self.ask
-        else:
-            raise ValueError(f'Invalid side {side}')
+            book[level - 1][entry_idx] = value
 
     @classmethod
     def from_json(cls, json_message: str | bytes | bytearray | dict) -> OrderBook:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
         dtype = json_dict.pop('dtype', None)
         if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
-        ticker = json_dict['ticker']
-        timestamp = json_dict['timestamp']
-        self = cls(ticker=ticker, timestamp=timestamp)
-
-        for log in json_dict.pop('bid'):
-            price = log[0]
-            volume = log[1]
-            self.bid.add_entry(price=price, volume=volume)
-
-        for log in json_dict.pop('ask'):
-            price = log[0]
-            volume = log[1]
-            self.ask.add_entry(price=price, volume=volume)
+        self = cls(**json_dict)
+        return self
 
-        self.additional.update(json_dict.get('additional', {}))
+    def to_list(self) -> list[float | int | str | bool]:
+        min_length = min(len(self.bid), len(self.ask))
+        r = ([self.__class__.__name__, self.ticker, self.timestamp]
+             + [value for entry in self.bid[:min_length] for value in entry]
+             + [value for entry in self.ask[:min_length] for value in entry])
 
-        return self
+        return r
 
-    @property
-    def max_level(self) -> int:
-        return max(len(self.bid), len(self.ask))
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> OrderBook:
+        dtype, ticker, timestamp = data_list[:3]
+        bid_data, ask_data = np.array(data_list[3:]).reshape(2, -1).tolist()
+        bid = np.array(bid_data).reshape(-1, 3).tolist()
+        ask = np.array(ask_data).reshape(-1, 3).tolist()
 
-    @property
-    def market_time(self):
-        return datetime.datetime.fromtimestamp(self.timestamp)
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        return cls(
+            ticker=ticker,
+            timestamp=timestamp,
+            bid=bid,
+            ask=ask
+        )
 
     @property
     def market_price(self):
-        """
-        Mid-price for a order book snapshot
-        :return: float
-        """
-        if np.isfinite(self.best_bid_price) and self.best_bid_price != 0 and np.isfinite(self.best_ask_price) and self.best_ask_price != 0:
-            return (self.best_bid_price + self.best_ask_price) / 2
-        else:
-            return np.nan
+        return self.mid_price
 
     @property
     def mid_price(self):
-        return self.market_price
+        if math.isfinite(self.best_bid_price) and math.isfinite(self.best_ask_price):
+            return (self.best_bid_price + self.best_ask_price) / 2
+        else:
+            return math.nan
 
     @property
     def spread(self):
-        if np.isfinite(self.best_bid_price) and self.best_bid_price != 0 and np.isfinite(self.best_ask_price) and self.best_ask_price != 0:
+        if math.isfinite(self.best_bid_price) and math.isfinite(self.best_ask_price):
             return self.best_ask_price - self.best_bid_price
         else:
-            return np.nan
+            return math.nan
 
     @property
     def spread_pct(self):
-        if np.isfinite(self.best_bid_price) and self.best_bid_price != 0 and np.isfinite(self.best_ask_price) and self.best_ask_price != 0:
-            return (self.best_ask_price - self.best_bid_price) / self.mid_price
+        if self.mid_price != 0:
+            return self.spread / self.mid_price
         else:
-            return np.nan
+            return np.inf
+
+    @property
+    def bid(self) -> Book:
+        book = self.Book(side=1)
+        for price, volume, *_ in self['bid']:
+            book.add(price=price, volume=volume)
+        book.sort()
+        return book
+
+    @property
+    def ask(self) -> Book:
+        book = self.Book(side=-1)
+        for price, volume, *_ in self['ask']:
+            book.add(price=price, volume=volume)
+        book.sort()
+        return book
 
     @property
     def best_bid_price(self):
-        if self.bid.price:
-            return self.bid.price[0]
+        if book := self.bid:
+            return book[0][0]
         else:
-            return np.nan
+            return math.nan
 
     @property
     def best_ask_price(self):
-        if self.ask.price:
-            return self.ask.price[0]
+        if book := self.ask:
+            return book[0][0]
         else:
-            return np.nan
+            return math.nan
 
     @property
     def best_bid_volume(self):
-        if self.bid.volume:
-            return self.bid.volume[0]
+        if book := self.bid:
+            return book[0][1]
         else:
-            return np.nan
+            return math.nan
 
     @property
     def best_ask_volume(self):
-        if self.ask.volume:
-            return self.ask.volume[0]
+        if book := self.ask:
+            return book[0][1]
         else:
-            return np.nan
+            return math.nan
 
 
 class BarData(MarketData):
     def __init__(
             self, *,
             ticker: str,
-            timestamp: float = None,  # the bar end timestamp
-            bar_start_time: datetime.datetime | datetime.date,
-            bar_span: datetime.timedelta,
+            timestamp: float,  # the bar end timestamp
+            start_timestamp: float = None,
+            bar_span: datetime.timedelta = None,
             high_price: float = math.nan,
             low_price: float = math.nan,
             open_price: float = math.nan,
             close_price: float = math.nan,
             volume: float = 0.,
             notional: float = 0.,
             trade_count: int = 0,
             **kwargs
     ):
-        """
-        store bar data
-        :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
-        :param high_price: max traded price of the given time frame
-        :param low_price: min traded price of the given time frame
-        :param open_price: trading price at the start of the bar
-        :param close_price: trading price at the end of the bar
-        :param bar_start_time: datetime.date for a daily bar or datetime.datetime for more detailed bar
-        :param bar_span: the length of the given time frame
-        :param volume: sum of traded volume at the given time frame
-        :param notional: sum of traded notional, or turnover
-        :param trade_count: number of trades happened during the time frame
-        """
-
-        if timestamp is None:
-            if isinstance(bar_start_time, datetime.datetime):
-                timestamp = (bar_start_time + bar_span).timestamp()
-            else:
-                LOGGER.warning('Auto-calculate timestamp of daily bar is not recommended')
-                timestamp = datetime.datetime.combine(bar_start_time, datetime.time.max).timestamp()
-
-        super().__init__(
-            ticker=ticker,
-            timestamp=timestamp
+        super().__init__(ticker=ticker, timestamp=timestamp, **kwargs)
+        self.update(
+            high_price=high_price,
+            low_price=low_price,
+            open_price=open_price,
+            close_price=close_price,
+            volume=volume,
+            notional=notional,
+            trade_count=trade_count
         )
 
-        self.high_price = float(high_price)
-        self.low_price = float(low_price)
-        self.open_price = float(open_price)
-        self.close_price = float(close_price)
-        self.bar_start_time = bar_start_time
-        self.bar_span = bar_span
-        self.volume = float(volume)
-        self.notional = float(notional)
-        self.trade_count = int(trade_count)
-        self.additional = {}
-
-        self.additional.update(kwargs)
+        if bar_span is None and start_timestamp is None:
+            raise ValueError('Must assign ether start_timestamp or bar_span or both.')
+        elif start_timestamp is None:
+            # self['start_timestamp'] = timestamp - bar_span.total_seconds()
+            if isinstance(bar_span, datetime.timedelta):
+                self['bar_span'] = bar_span.total_seconds()
+            elif isinstance(bar_span, (int, float)):
+                self['bar_span'] = bar_span
+            else:
+                raise ValueError(f'Invalid bar_span, expect int, float or timedelta, got {bar_span}')
+        elif bar_span is None:
+            self['start_timestamp'] = start_timestamp
+            # self['bar_span'] = timestamp - start_timestamp
+        else:
+            self['start_timestamp'] = start_timestamp
+
+            if isinstance(bar_span, datetime.timedelta):
+                self['bar_span'] = bar_span.total_seconds()
+            elif isinstance(bar_span, (int, float)):
+                self['bar_span'] = bar_span
+            else:
+                raise ValueError(f'Invalid bar_span, expect int, float or timedelta, got {bar_span}')
 
     def __repr__(self):
-        return '<BarData>{}'.format(self.__dict__)
-
-    def __eq__(self, other):
-        if isinstance(other, BarData):
-            return self.__repr__() == other.__repr__()
-        else:
-            return False
-
-    def __lt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        assert other.bar_span == self.bar_span, 'BarSpan not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.bar_start_time < other.bar_start_time
-
-    def __gt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        assert other.bar_span == self.bar_span, 'BarSpan not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.bar_start_time > other.bar_start_time
-
-    def __le__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        assert other.bar_span == self.bar_span, 'BarSpan not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.bar_start_time <= other.bar_start_time
-
-    def __ge__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        assert other.bar_span == self.bar_span, 'BarSpan not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.bar_start_time >= other.bar_start_time
-
-    def __str__(self):
-        if type(self.bar_start_time) is datetime.date:
-            return f'<BarData>([{self.bar_start_time:%Y-%m-%d}] {self.ticker} Opened @ {self.open_price}; Closed @ {self.close_price}; Lasted {self.bar_span})'
-        else:
-            return f'<BarData>([{self.bar_start_time:%Y-%m-%d %H:%M:%S}] {self.ticker} Opened @ {self.open_price}; Closed @ {self.close_price}; Lasted {self.bar_span})'
-
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'market_time': (self.market_time.__class__.__name__, self.market_time.strftime('%Y-%m-%d %H:%M:%S')),
-            'bar_span': self.bar_span.total_seconds(),
-            'high_price': self.high_price,
-            'low_price': self.low_price,
-            'open_price': self.open_price,
-            'close_price': self.close_price,
-            'volume': self.volume,
-            'notional': self.notional,
-            'trade_count': self.trade_count
-        }
-
-        if self.additional:
-            data_dict['additional'] = self.additional
-
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+        return f'<BarData>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker}, open={self.open_price}, close={self.close_price}, high={self.high_price}, low={self.low_price})'
 
     @classmethod
     def from_json(cls, json_message: str | bytes | bytearray | dict) -> BarData:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
         dtype = json_dict.pop('dtype', None)
         if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        self = cls(**json_dict)
+        return self
 
-        bar_start_time = json_dict.pop('market_time')
+    def to_list(self) -> list[float | int | str | bool]:
+        return [self.__class__.__name__,
+                self.ticker,
+                self.timestamp,
+                self.high_price,
+                self.low_price,
+                self.open_price,
+                self.close_price,
+                self.get('start_timestamp'),
+                self.get('bar_span'),
+                self.volume,
+                self.notional,
+                self.trade_count]
 
-        self = cls(
-            ticker=json_dict.pop('ticker'),
-            high_price=json_dict.pop('high_price'),
-            low_price=json_dict.pop('low_price'),
-            open_price=json_dict.pop('open_price'),
-            close_price=json_dict.pop('close_price'),
-            bar_start_time=datetime.datetime.strptime(bar_start_time[1], '%Y-%m-%d %H:%M:%S'),
-            bar_span=datetime.timedelta(seconds=json_dict.pop('bar_span')),
-            volume=json_dict.pop('volume'),
-            notional=json_dict.pop('notional'),
-            trade_count=json_dict.pop('trade_count')
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> BarData:
+        (dtype, ticker, timestamp, high_price, low_price, open_price, close_price,
+         start_timestamp, bar_span, volume, notional, trade_count) = data_list
+
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        return cls(
+            ticker=ticker,
+            timestamp=timestamp,
+            high_price=high_price,
+            low_price=low_price,
+            open_price=open_price,
+            close_price=close_price,
+            start_timestamp=start_timestamp if start_timestamp else None,
+            bar_span=datetime.timedelta(bar_span) if bar_span else None,
+            volume=volume,
+            notional=notional,
+            trade_count=trade_count
         )
 
-        if bar_start_time[0] == 'date':
-            self.bar_start_time = self.bar_start_time.date()
+    @property
+    def high_price(self) -> float:
+        return self['high_price']
 
-        self.additional.update(json_dict.get('additional', {}))
+    @property
+    def low_price(self) -> float:
+        return self['low_price']
 
-        return self
+    @property
+    def open_price(self) -> float:
+        return self['open_price']
+
+    @property
+    def close_price(self) -> float:
+        return self['close_price']
+
+    @property
+    def bar_span(self) -> datetime.timedelta:
+        if 'bar_span' in self:
+            return datetime.timedelta(seconds=self['bar_span'])
+        else:
+            return datetime.timedelta(seconds=self['timestamp'] - self['start_timestamp'])
+
+    @property
+    def volume(self) -> float:
+        return self['volume']
+
+    @property
+    def notional(self) -> float:
+        return self['notional']
 
-    # noinspection PyPep8Naming, SpellCheckingInspection
     @property
-    def VWAP(self) -> float:
+    def trade_count(self) -> int:
+        return self['trade_count']
+
+    @property
+    def bar_start_time(self) -> datetime.datetime:
+        if 'start_timestamp' in self:
+            return datetime.datetime.fromtimestamp(self['start_timestamp'], tz=TIME_ZONE)
+        else:
+            return datetime.datetime.fromtimestamp(self['timestamp'] - self['bar_span'], tz=TIME_ZONE)
+
+    @property
+    def vwap(self) -> float:
         if self.volume != 0:
             return self.notional / self.volume
         else:
-            LOGGER.warning('[{}] {} Volume data not available, using close_price as default VWAP value'.format(self.bar_start_time, self.ticker))
+            LOGGER.warning(f'[{self.market_time}] {self.ticker} Volume data not available, using close_price as default VWAP value')
             return self.close_price
 
     @property
     def is_valid(self, verbose=False) -> bool:
         try:
             assert type(self.ticker) is str, '{} Invalid ticker'.format(str(self))
-            assert np.isfinite(self.high_price), '{} Invalid high_price'.format(str(self))
-            assert np.isfinite(self.low_price), '{} Invalid low_price'.format(str(self))
-            assert np.isfinite(self.open_price), '{} Invalid open_price'.format(str(self))
-            assert np.isfinite(self.close_price), '{} Invalid close_price'.format(str(self))
-            assert np.isfinite(self.volume), '{} Invalid volume'.format(str(self))
-            assert np.isfinite(self.notional), '{} Invalid notional'.format(str(self))
-            assert np.isfinite(self.trade_count), '{} Invalid trade_count'.format(str(self))
+            assert math.isfinite(self.high_price), '{} Invalid high_price'.format(str(self))
+            assert math.isfinite(self.low_price), '{} Invalid low_price'.format(str(self))
+            assert math.isfinite(self.open_price), '{} Invalid open_price'.format(str(self))
+            assert math.isfinite(self.close_price), '{} Invalid close_price'.format(str(self))
+            assert math.isfinite(self.volume), '{} Invalid volume'.format(str(self))
+            assert math.isfinite(self.notional), '{} Invalid notional'.format(str(self))
+            assert math.isfinite(self.trade_count), '{} Invalid trade_count'.format(str(self))
             assert isinstance(self.bar_start_time, (datetime.datetime, datetime.date)), '{} Invalid bar_start_time'.format(str(self))
             assert isinstance(self.bar_span, datetime.timedelta), '{} Invalid bar_span'.format(str(self))
 
             return True
         except AssertionError as e:
             if verbose:
                 LOGGER.warning(str(e))
             return False
 
     @property
-    def market_time(self):
-        return self.bar_end_time
-
-    @property
     def market_price(self):
         """
         close price for a BarData
         :return: float
         """
         return self.close_price
 
@@ -1005,805 +877,646 @@
             return 'Over-Minute'
         elif self.bar_span == datetime.timedelta(minutes=1):
             return 'Minute'
         else:
             return 'Sub-Minute'
 
     @property
-    def bar_end_time(self):
+    def bar_end_time(self) -> datetime.datetime | datetime.date:
         if self.bar_type == 'Daily':
-            return self.bar_start_time
+            return self.market_time.date()
         else:
-            return self.bar_start_time + self.bar_span
+            return self.market_time
 
 
 class TickData(MarketData):
     def __init__(
             self, *,
             ticker: str,
+            timestamp: float,
             last_price: float,
-            market_time: datetime.datetime = None,
-            timestamp: float = None,
+            bid_price: float = None,
+            bid_volume: float = None,
+            ask_price: float = None,
+            ask_volume: float = None,
             order_book: OrderBook = None,
-            total_traded_volume: float = float('nan'),
-            total_traded_notional: float = float('nan'),
+            total_traded_volume: float = 0.,
+            total_traded_notional: float = 0.,
             total_trade_count: int = 0,
             **kwargs
     ):
-        """
-        store tick data
-        :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
-        :param market_time: datetime.datetime of the tick data
-        :param last_price: last traded price
-        :param total_traded_volume: total traded volume no after this tick, use float to compatible with crypto
-        :param total_traded_notional: total traded notional no after this tick
-        :param kwargs: additional OrderBook data
-        :keyword bid_price: bid 1 price
-        :keyword ask_price: ask 1 price
-        :keyword bid_volume: bid 1 volume
-        :keyword ask_volume: ask 1 volume
-        """
+        super().__init__(ticker=ticker, timestamp=timestamp, **kwargs)
 
-        super().__init__(
-            ticker=ticker,
-            timestamp=market_time.timestamp() if timestamp is None else timestamp
+        self.update(
+            last_price=last_price,
+            total_traded_volume=total_traded_volume,
+            total_traded_notional=total_traded_notional,
+            total_trade_count=total_trade_count,
         )
 
-        if 'bid_price' in kwargs:
-            kwargs['bid_price_1'] = kwargs.pop('bid_price')
+        if bid_price is not None and math.isfinite(bid_price):
+            self['bid_price'] = bid_price
 
-        if 'ask_price' in kwargs:
-            kwargs['ask_price_1'] = kwargs.pop('ask_price')
+        if bid_volume is not None and math.isfinite(bid_volume):
+            self['bid_volume'] = bid_volume
 
-        if 'bid_volume' in kwargs:
-            kwargs['bid_volume_1'] = kwargs.pop('bid_volume')
+        if ask_price is not None and math.isfinite(ask_price):
+            self['ask_price'] = ask_price
 
-        if 'ask_volume' in kwargs:
-            kwargs['ask_volume_1'] = kwargs.pop('ask_volume')
+        if ask_volume is not None and math.isfinite(ask_volume):
+            self['ask_volume'] = ask_volume
 
         if order_book is not None:
-            self.order_book = order_book
-        else:
-            self.order_book = OrderBook(ticker=ticker, market_time=market_time, timestamp=timestamp)
+            self['order_book'] = order_book
 
-        self.last_price = float(last_price)
-        self.total_traded_volume = float(total_traded_volume)
-        self.total_traded_notional = float(total_traded_notional)
-        self.total_trade_count = int(total_trade_count)
-
-        self.order_book.update(**kwargs)
+        if kwargs:
+            self['additional'] = dict(kwargs)
 
     @property
-    def market_time(self):
-        return self.order_book.market_time
+    def level_2(self) -> OrderBook | None:
+        if 'order_book' in self:
+            return OrderBook(**self['order_book'])
+        else:
+            return None
 
     @property
-    def level_2(self):
-        return self.order_book
+    def last_price(self) -> float:
+        return self['last_price']
 
     @property
-    def bid_price(self):
-        return self.order_book.best_bid_price
+    def bid_price(self) -> float | None:
+        return self.get('bid_price')
 
     @property
-    def ask_price(self):
-        return self.order_book.best_ask_price
+    def ask_price(self) -> float | None:
+        return self.get('ask_price')
 
     @property
-    def bid_volume(self):
-        return self.order_book.best_bid_volume
+    def bid_volume(self) -> float | None:
+        return self.get('bid_volume')
 
     @property
-    def ask_volume(self):
-        return self.order_book.best_ask_volume
+    def ask_volume(self) -> float | None:
+        return self.get('ask_volume')
 
-    def __repr__(self):
-        return '<TickData>{}'.format({key: item.__dict__ if key == 'level_2' else item for key, item in self.__dict__.items()})
-
-    def __eq__(self, other):
-        if isinstance(other, TickData):
-            return self.__repr__() == other.__repr__()
-        else:
-            return False
-
-    def __lt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time < other.market_time
-
-    def __gt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time > other.market_time
-
-    def __le__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time <= other.market_time
-
-    def __ge__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time >= other.market_time
-
-    def __str__(self):
-        return f'<TickData>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker} {{Bid: ({self.bid_price}: {self.bid_volume}), Ask: ({self.ask_price}: {self.ask_volume}), Last: {self.last_price}}})'
+    @property
+    def total_traded_volume(self) -> float:
+        return self['total_traded_volume']
 
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'timestamp': self.timestamp,
-            'last_price': self.last_price,
-            'total_traded_volume': self.total_traded_volume,
-            'total_traded_notional': self.total_traded_notional,
-            'total_trade_count': self.total_trade_count,
-            'bid': [(entry.price, entry.volume) for entry in self.order_book.bid],
-            'ask': [(entry.price, entry.volume) for entry in self.order_book.ask],
-        }
+    @property
+    def total_traded_notional(self) -> float:
+        return self['total_traded_notional']
 
-        if self.additional:
-            data_dict['additional'] = self.additional
+    @property
+    def total_trade_count(self) -> float:
+        return self['total_trade_count']
 
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+    def __repr__(self):
+        return f'<TickData>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker}, bid={self.bid_price}, ask={self.ask_price})'
 
     @classmethod
     def from_json(cls, json_message: str | bytes | bytearray | dict) -> TickData:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
         dtype = json_dict.pop('dtype', None)
         if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        self = cls(**json_dict)
+        return self
+
+    def to_list(self) -> list[float | int | str | bool]:
+        """
+        note that to_list WILL NOT retain orderbook info.
+        to save all info, use to_json instead.
+        """
+        return [self.__class__.__name__,
+                self.ticker,
+                self.timestamp,
+                self.last_price,
+                self.bid_price,
+                self.bid_volume,
+                self.ask_price,
+                self.ask_volume,
+                self.total_traded_volume,
+                self.total_traded_notional,
+                self.total_trade_count]
+
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> TickData:
+        (dtype, ticker, timestamp, last_price,
+         bid_price, bid_volume, ask_price, ask_volume,
+         total_traded_volume, total_traded_notional, total_trade_count) = data_list
 
-        ticker = json_dict.pop('ticker')
-        timestamp = json_dict.pop('timestamp')
-        order_book = OrderBook(ticker=ticker, timestamp=timestamp)
-
-        for log in json_dict.pop('bid'):
-            price = log[0]
-            volume = log[1]
-            order_book.bid.add_entry(price=price, volume=volume)
-
-        for log in json_dict.pop('ask'):
-            price = log[0]
-            volume = log[1]
-            order_book.ask.add_entry(price=price, volume=volume)
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
-        self = cls(
+        kwargs = {}
+
+        if bid_price is not None:
+            kwargs['bid_price'] = bid_price
+
+        if ask_price is not None:
+            kwargs['ask_price'] = ask_price
+
+        if bid_volume is not None:
+            kwargs['bid_volume'] = bid_volume
+
+        if ask_volume is not None:
+            kwargs['ask_volume'] = ask_volume
+
+        return cls(
             ticker=ticker,
             timestamp=timestamp,
-            last_price=json_dict.pop('last_price'),
-            order_book=order_book,
-            total_traded_volume=json_dict.pop('total_traded_volume'),
-            total_traded_notional=json_dict.pop('total_traded_notional'),
-            total_trade_count=json_dict.pop('total_trade_count'),
+            last_price=last_price,
+            total_traded_volume=total_traded_volume,
+            total_traded_notional=total_traded_notional,
+            total_trade_count=total_trade_count,
+            **kwargs
         )
 
-        self.additional.update(json_dict.get('additional', {}))
-
-        return self
-
     @property
-    def mid_price(self):
-        return self.order_book.mid_price
+    def mid_price(self) -> float:
+        return (self.bid_price + self.ask_price) / 2
 
     @property
     def market_price(self) -> float:
-        """
-        Last price for a TickData
-        :return:
-        """
         return self.last_price
 
-    @property
-    def additional(self):
-        return self.order_book.additional
-
 
-class TradeData(MarketData):
+class TransactionData(MarketData):
     def __init__(
             self, *,
             ticker: str,
-            trade_price: float,
-            trade_volume: float,
-            trade_time: datetime.datetime = None,
-            timestamp: float = None,
+            price: float,
+            volume: float,
+            timestamp: float,
             side: int | float | str | TransactionSide = 0,
-            multiplier: float = 1,
+            multiplier: float = None,
             notional: float = None,
+            transaction_id: str | int = None,
+            buy_id: str | int = None,
+            sell_id: str | int = None,
             **kwargs
     ):
-        """
-        store trade data
-        :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
-        :param trade_time: datetime.datetime of the trade
-        :param trade_price: trade price
-        :param trade_volume: use float to compatible with crypto
-        :param side: TransactionSide indicating which side of the order book get taken
-        :param multiplier: multiplier for contract trade data
-        """
-
-        super().__init__(
-            ticker=ticker,
-            timestamp=trade_time.timestamp() if timestamp is None else timestamp
-        )
-
-        self.price = float(trade_price)
-        self.volume = float(trade_volume)
-        self.trade_time = datetime.datetime.fromtimestamp(self.timestamp) if trade_time is None else trade_time
-        self.side = TransactionSide(side)
-        self.multiplier = float(multiplier)
-        self.notional = self.price * self.volume * self.multiplier if notional is None else notional
-        self.additional = {}
-
-        self.additional.update(**kwargs)
-
-    def __repr__(self):
-        return '<TradeData>{}'.format({key: item.name if key == 'side' else item for key, item in self.__dict__.items()})
-
-    def __eq__(self, other):
-        if isinstance(other, TradeData):
-            return self.__repr__() == other.__repr__()
-        else:
-            return False
-
-    def __lt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.trade_time < other.trade_time
-
-    def __gt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.trade_time > other.trade_time
-
-    def __le__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.trade_time <= other.trade_time
-
-    def __ge__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.trade_time >= other.trade_time
+        super().__init__(ticker=ticker, timestamp=timestamp, **kwargs)
 
-    def __str__(self):
-        return '<TradeData>([{:%Y-%m-%d %H:%M:%S}] {} {} {:.2f} @ {:.2f} notional {:.2f})'.format(self.trade_time, self.ticker, self.side.name, self.volume, self.price, self.notional)
+        self['price'] = price
+        self['volume'] = volume
+        self['side'] = int(side) if isinstance(side, (int, float)) else TransactionSide(side).value
 
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
+        if multiplier is not None and math.isfinite(multiplier):
+            self['multiplier'] = multiplier
 
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'timestamp': self.timestamp,
-            'side': self.side.value,
-            'volume': self.volume,
-            'price': self.price,
-
-        }
+        if notional is not None and math.isfinite(notional):
+            self['notional'] = notional
 
-        if self.multiplier != 1:
-            data_dict['multiplier'] = self.multiplier
+        if transaction_id is not None:
+            self['transaction_id'] = transaction_id
 
-        if self.notional != self.price * self.volume * self.multiplier:
-            data_dict['notional'] = self.notional
+        if buy_id is not None:
+            self['buy_id'] = buy_id
 
-        if self.additional:
-            data_dict['additional'] = self.additional
+        if sell_id is not None:
+            self['sell_id'] = sell_id
 
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+    def __repr__(self):
+        return f'<TransactionData>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.side.side_name} {self.ticker}, price={self.price}, volume={self.volume})'
 
     @classmethod
-    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TradeData:
+    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TransactionData:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
         dtype = json_dict.pop('dtype', None)
         if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
-        self = cls(
-            ticker=json_dict.pop('ticker'),
-            side=TransactionSide(json_dict.pop('side')),
-            trade_volume=json_dict.pop('volume'),
-            trade_price=json_dict.pop('price'),
-            timestamp=json_dict.pop('timestamp'),
-        )
+        self = cls(**json_dict)
+        return self
 
-        if 'multiplier' in json_dict:
-            self.multiplier = json_dict['multiplier']
+    def to_list(self) -> list[float | int | str | bool]:
+        return [self.__class__.__name__,
+                self.ticker,
+                self.timestamp,
+                self.price,
+                self.volume,
+                self['side'],
+                self.get('multiplier'),
+                self.get('notional'),
+                self.get('transaction_id'),
+                self.get('buy_id'),
+                self.get('sell_id')]
 
-        if 'notional' in json_dict:
-            self.notional = json_dict['notional']
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> TransactionData:
+        (dtype, ticker, timestamp, price, volume, side,
+         multiplier, notional, transaction_id, buy_id, sell_id) = data_list
 
-        self.additional.update(json_dict.get('additional', {}))
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
-        return self
+        kwargs = {}
+
+        if multiplier is not None:
+            kwargs['multiplier'] = multiplier
+
+        if notional in kwargs:
+            kwargs['notional'] = notional
+
+        if transaction_id in kwargs:
+            kwargs['transaction_id'] = transaction_id
+
+        if buy_id in kwargs:
+            kwargs['buy_id'] = buy_id
+
+        if sell_id in kwargs:
+            kwargs['sell_id'] = sell_id
+
+        return cls(
+            ticker=ticker,
+            timestamp=timestamp,
+            price=price,
+            volume=volume,
+            side=side,
+            **kwargs
+        )
 
-    @staticmethod
-    def merge(trade_data_list: list[TradeData]) -> TradeData | None:
+    @classmethod
+    def merge(cls, trade_data_list: list[TransactionData]) -> TransactionData | None:
         if not trade_data_list:
             return None
 
         ticker = trade_data_list[0].ticker
         assert all([trade.ticker == ticker for trade in trade_data_list]), 'input contains trade data of multiple ticker'
         timestamp = max([trade.timestamp for trade in trade_data_list])
         sum_volume = sum([trade.volume * trade.side.sign for trade in trade_data_list])
         sum_notional = sum([trade.notional * trade.side.sign for trade in trade_data_list])
         trade_side_sign = np.sign(sum_volume) if sum_volume != 0 else 1
 
         if sum_notional == 0:
             trade_price = 0
+        elif sum_volume == 0:
+            trade_price = math.nan
         else:
-            trade_price = np.divide(sum_notional, sum_volume)
+            trade_price = sum_notional / sum_volume if sum_volume else math.inf * np.sign(sum_notional)
 
-        trade_volume = sum_volume * trade_side_sign
         trade_side = TransactionSide(trade_side_sign)
-        trade_notional = sum_notional * trade_side_sign
+        trade_volume = abs(sum_volume)
+        trade_notional = abs(sum_notional)
 
-        merged_trade_data = TradeData(
+        merged_trade_data = cls(
             ticker=ticker,
             timestamp=timestamp,
-            trade_price=trade_price,
-            trade_volume=trade_volume,
-            side=trade_side
+            side=trade_side,
+            price=trade_price,
+            volume=trade_volume,
+            notional=trade_notional
         )
-        merged_trade_data.notional = trade_notional
 
         return merged_trade_data
 
     @property
-    def market_time(self):
-        return self.trade_time
+    def price(self) -> float:
+        return self['price']
 
     @property
-    def market_price(self) -> float:
-        """
-        Trade Price for a TradeData
-        :return:
-        """
-        return self.price
+    def volume(self) -> float:
+        return self['volume']
 
     @property
-    def flow(self):
-        return self.side.sign * self.volume
-
+    def side(self) -> TransactionSide:
+        return TransactionSide(self['side'])
 
-class TransactionData(MarketData):
-    def __init__(
-            self, *,
-            ticker: str,
-            price: float,
-            volume: float,
-            transaction_time: datetime.datetime = None,
-            timestamp: float = None,
-            side: int | float | str | TransactionSide = 0,
-            multiplier: float = 1,
-            **kwargs
-    ):
-        """
-        store trade data
-        :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
-        :param trade_time: datetime.datetime of the trade
-        :param trade_price: trade price
-        :param trade_volume: use float to compatible with crypto
-        :param side: TransactionSide indicating which side of the order book get taken
-        :param multiplier: multiplier for contract trade data
-        """
+    @property
+    def multiplier(self) -> float:
+        return self.get('multiplier', 1.)
 
-        super().__init__(
-            ticker=ticker,
-            timestamp=transaction_time.timestamp() if timestamp is None else timestamp
-        )
+    @property
+    def transaction_id(self) -> int | str | None:
+        return self.get('transaction_id', None)
 
-        self.price = float(price)
-        self.volume = float(volume)
-        self.transaction_time = datetime.datetime.fromtimestamp(self.timestamp) if transaction_time is None else transaction_time
-        self.side = TransactionSide(side)
-        self.multiplier = float(multiplier)
-        self.notional = self.price * self.volume * self.multiplier
+    @property
+    def buy_id(self) -> int | str | None:
+        return self.get('buy_id', None)
 
-        if transaction_time is None and timestamp is None:
-            raise ValueError('Must assign ether transaction_time or timestamp')
+    @property
+    def sell_id(self) -> int | str | None:
+        return self.get('sell_id', None)
 
-        for name, value in kwargs.items():
-            setattr(self, name, value)
+    @property
+    def notional(self) -> float:
+        return self.get('notional', self.price * self.volume * self.multiplier)
 
-    def __repr__(self):
-        return '<TradeData>{}'.format({key: item.name if key == 'side' else item for key, item in self.__dict__.items()})
+    @property
+    def market_price(self) -> float:
+        return self.price
 
-    def __eq__(self, other):
-        if isinstance(other, TradeData):
-            return self.__repr__() == other.__repr__()
-        else:
-            return False
+    @property
+    def flow(self):
+        return self.side.sign * self.volume
 
-    def __lt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time < other.market_time
 
-    def __gt__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time > other.market_time
-
-    def __le__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time <= other.market_time
-
-    def __ge__(self, other):
-        assert isinstance(other, self.__class__), 'Can not compare {} with {}'.format(other.__class__.__name__, self.__class__.__name__)
-        assert other.ticker == self.ticker, 'Ticker not match! Can not compare TradeData of {} with {}'.format(other.ticker, self.ticker)
-        return self.market_time >= other.market_time
+class TradeData(TransactionData):
+    """
+    TradeData is an alias of TransactionData
+    TradeData can be initialized with 'trade_price' instead of 'price'; 'trade_volume' instead of 'volume'.
+    The corresponding properties are added.
+    """
 
-    def __str__(self):
-        return '<TransactionData>([{:%Y-%m-%d %H:%M:%S}] {} {} {:.2f} @ {:.2f} notional {:.2f})'.format(self.market_time, self.ticker, self.side.name, self.volume, self.price, self.notional)
+    def __init__(self, **kwargs):
+        if 'trade_price' in kwargs:
+            kwargs['price'] = kwargs.pop('trade_price')
 
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
+        if 'trade_volume' in kwargs:
+            kwargs['volume'] = kwargs.pop('trade_volume')
 
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'timestamp': self.timestamp,
-            'side': self.side.value
-        }
+        super().__init__(**kwargs)
 
-        data_dict.update({key: value for key, value in self.__dict__.items() if key not in ['_ticker', 'side', 'timestamp']})
+    @property
+    def trade_price(self) -> float:
+        return self['price']
 
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+    @property
+    def trade_volume(self) -> float:
+        return self['volume']
 
     @classmethod
-    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TransactionData:
-        if isinstance(json_message, dict):
-            json_dict = json_message
-        else:
-            json_dict = json.loads(json_message)
+    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TradeData:
+        # noinspection PyTypeChecker
+        return super(TradeData, cls).from_json(json_message=json_message)
 
-        dtype = json_dict.pop('dtype', None)
-        if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> TradeData:
+        # noinspection PyTypeChecker
+        return super(TradeData, cls).from_list(data_list=data_list)
 
-        self = cls(
-            ticker=json_dict.pop('ticker'),
-            side=TransactionSide(json_dict.pop('side')),
-            volume=json_dict.pop('volume'),
-            price=json_dict.pop('price'),
-            timestamp=json_dict.pop('timestamp'),
-        )
 
-        for key, value in json_dict.items():
-            setattr(self, key, value)
+class _MarketDataMemoryBuffer(object, metaclass=abc.ABCMeta):
+    def __init__(self):
+        self.dtype = RawArray(c_wchar, 16)
+        self.ticker = RawArray(c_wchar, 32)  # max length of ticker is 32
+        self.timestamp = RawValue(c_double)
+
+    def update(self, market_data: MarketData):
+        self.dtype.value = market_data.__class__.__name__
+        self.ticker.value = market_data['ticker']
+        self.timestamp.value = market_data['timestamp']
 
-        return self
+    @abc.abstractmethod
+    def to_market_data(self) -> MarketData:
+        ...
 
-    @staticmethod
-    def merge(trade_data_list: list[TransactionData]) -> TransactionData | None:
-        if not trade_data_list:
-            return None
 
-        ticker = trade_data_list[0].ticker
-        assert all([trade.ticker == ticker for trade in trade_data_list]), 'input contains trade data of multiple ticker'
-        trade_time = max([trade.market_time for trade in trade_data_list])
-        sum_volume = sum([trade.volume * trade.side.sign for trade in trade_data_list])
-        sum_notional = sum([trade.notional * trade.side.sign for trade in trade_data_list])
-        trade_side_sign = np.sign(sum_volume) if sum_volume != 0 else 1
+class OrderBookBuffer(_MarketDataMemoryBuffer):
+    def __init__(self, max_level: int = 20):
+        super().__init__()
 
-        if sum_notional == 0:
-            trade_price = 0
-        else:
-            trade_price = np.divide(sum_notional, sum_volume)
+        self.max_level = max_level
 
-        trade_volume = sum_volume * trade_side_sign
-        trade_side = TransactionSide(trade_side_sign)
-        trade_notional = sum_notional * trade_side_sign
+        self.bid = [(RawValue(c_double), RawValue(c_double), RawValue(c_ulong)) for _ in range(self.max_level)]
+        self.ask = [(RawValue(c_double), RawValue(c_double), RawValue(c_ulong)) for _ in range(self.max_level)]
 
-        merged_trade_data = TransactionData(
-            ticker=ticker,
-            market_time=trade_time,
-            price=trade_price,
-            volume=trade_volume,
-            side=trade_side
-        )
-        merged_trade_data.notional = trade_notional
+    def update(self, market_data: OrderBook):
+        super().update(market_data=market_data)
 
-        return merged_trade_data
+        bid = market_data['bid']
+        ask = market_data['ask']
 
-    @property
-    def market_time(self):
-        if self.transaction_time:
-            return self.transaction_time
-        else:
-            return datetime.datetime.fromtimestamp(self.timestamp)
+        for i in range(self.max_level):
+            bid_memory_array = self.bid[i]
+            ask_memory_array = self.ask[i]
 
-    @property
-    def market_price(self) -> float:
-        """
-        Trade Price for a TradeData
-        :return:
-        """
-        return self.price
+            if i < len(bid):
+                for bid_entry_value, bid_memory in zip(bid[i], bid_memory_array):
+                    bid_memory.value = bid_entry_value
+            else:
+                for bid_memory in bid_memory_array:
+                    bid_memory.value = 0
 
-    @property
-    def flow(self):
-        return self.side.sign * self.volume
+            if i < len(ask):
+                for ask_entry_value, ask_memory in zip(ask[i], ask_memory_array):
+                    ask_memory.value = ask_entry_value
+            else:
+                for ask_memory in ask_memory_array:
+                    ask_memory.value = 0.
 
+    def to_market_data(self) -> OrderBook:
+        bid, ask = [], []
 
-class OrderBookDiff(MarketData):
-    def __init__(
-            self,
-            ticker: str,
-            market_time: datetime.datetime = None,
-            timestamp: float = None,
-            bid_diff=None,
-            ask_diff=None,
-            **kwargs):
+        for i in range(self.max_level):
+            bid_memory_array = self.bid[i]
+            ask_memory_array = self.ask[i]
 
-        super().__init__(
-            ticker=ticker,
-            timestamp=market_time.timestamp() if timestamp is None else timestamp
-        )
+            bid_price, bid_volume, bid_n_orders = [_.value for _ in bid_memory_array]
+            ask_price, ask_volume, ask_n_orders = [_.value for _ in ask_memory_array]
 
-        self.bid_diff = {} if bid_diff is None else dict(bid_diff)
-        self.ask_diff = {} if ask_diff is None else dict(ask_diff)
+            if bid_volume:
+                bid.append([bid_price, bid_volume, bid_n_orders])
 
-        self.additional = dict(**kwargs)
+            if ask_volume:
+                ask.append([ask_price, ask_volume, ask_n_orders])
 
-    def __repr__(self):
-        return f'<OrderBookDiff>{self.ticker}'
+            if bid_volume == ask_volume == 0:
+                break
 
-    def __str__(self):
-        return f'<OrderBookDiff>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker} with {len(self.bid_diff) + len(self.ask_diff)} diffs)'
+        order_book = OrderBook(
+            ticker=self.ticker.value,
+            timestamp=self.timestamp.value,
+            bid=bid,
+            ask=ask,
+        )
 
-    def to_json(self, fmt='str', **kwargs) -> str | dict:
+        return order_book
 
-        data_dict = {
-            'dtype': self.__class__.__name__,
-            'ticker': self.ticker,
-            'timestamp': self.timestamp,
-            'bid_diff': self.bid_diff,
-            'ask_diff': self.ask_diff,
-        }
 
-        if self.additional:
-            data_dict['additional'] = self.additional
+class BarDataBuffer(_MarketDataMemoryBuffer):
+    def __init__(self):
+        super().__init__()
+
+        self.start_timestamp = RawValue(c_double)
+        self.bar_span = RawValue(c_double)
+        self.high_price = RawValue(c_double)
+        self.low_price = RawValue(c_double)
+        self.open_price = RawValue(c_double)
+        self.close_price = RawValue(c_double)
+        self.volume = RawValue(c_double)
+        self.notional = RawValue(c_double)
+        self.trade_count = RawValue(c_longlong)
+
+    def update(self, market_data: BarData):
+        super().update(market_data=market_data)
+
+        self.start_timestamp.value = market_data['start_timestamp'] if 'start_timestamp' in market_data else math.nan
+        self.bar_span.value = market_data['bar_span'] if 'bar_span' in market_data else math.nan
+
+        self.high_price.value = market_data['high_price']
+        self.low_price.value = market_data['low_price']
+        self.open_price.value = market_data['open_price']
+        self.close_price.value = market_data['close_price']
+        self.volume.value = market_data['volume']
+        self.notional.value = market_data['notional']
+        self.trade_count.value = market_data['trade_count']
+
+    def to_market_data(self) -> BarData:
+        bar_data = BarData(
+            ticker=self.ticker.value,
+            timestamp=self.timestamp.value,
+            start_timestamp=self.start_timestamp.value if math.isfinite(self.start_timestamp.value) else None,
+            bar_span=self.bar_span.value if math.isfinite(self.bar_span.value) else None,
+            high_price=self.high_price.value,
+            low_price=self.low_price.value,
+            open_price=self.open_price.value,
+            close_price=self.close_price.value,
+            volume=self.volume.value,
+            notional=self.notional.value,
+            trade_count=self.trade_count.value
+        )
 
-        if fmt == 'dict':
-            return data_dict
-        else:
-            return json.dumps(data_dict, **kwargs)
+        return bar_data
 
-    @classmethod
-    def from_json(cls, json_message: str | bytes | bytearray | dict) -> OrderBookDiff:
-        if isinstance(json_message, dict):
-            json_dict = json_message
-        else:
-            json_dict = json.loads(json_message)
 
-        dtype = json_dict.pop('dtype', None)
-        if dtype is not None and dtype != cls.__name__:
-            raise TypeError(f'Invalid dtype {dtype}')
-
-        self = cls(
-            ticker=json_dict.pop('ticker'),
-            timestamp=json_dict.pop('timestamp'),
-            bid_diff=json_dict.pop('bid_diff'),
-            ask_diff=json_dict.pop('ask_diff'),
-            **json_dict.get('additional', {})
+class TickDataBuffer(_MarketDataMemoryBuffer):
+    def __init__(self):
+        super().__init__()
+
+        self.last_price = RawValue(c_double)
+        self.bid_price = RawValue(c_double)
+        self.bid_volume = RawValue(c_double)
+        self.ask_price = RawValue(c_double)
+        self.ask_volume = RawValue(c_double)
+        self.total_traded_volume = RawValue(c_double)
+        self.total_traded_notional = RawValue(c_double)
+        self.total_trade_count = RawValue(c_longlong)
+
+    def update(self, market_data: TickData):
+        """
+        note that the order book is not stored in shared memory.
+        use OrderBookShared to store the level2 data.
+        """
+        super().update(market_data=market_data)
+
+        self.last_price.value = market_data.last_price
+
+        self.bid_price.value = market_data['bid_price'] if 'bid_price' in market_data else math.nan
+        self.bid_volume.value = market_data['bid_volume'] if 'bid_volume' in market_data else math.nan
+        self.ask_price.value = market_data['ask_price'] if 'ask_price' in market_data else math.nan
+        self.ask_volume.value = market_data['ask_volume'] if 'ask_volume' in market_data else math.nan
+
+        self.total_traded_volume.value = market_data['total_traded_volume']
+        self.total_traded_notional.value = market_data['total_traded_notional']
+        self.total_trade_count.value = market_data['total_trade_count']
+
+    def to_market_data(self) -> TickData:
+        tick_data = TickData(
+            ticker=self.ticker.value,
+            timestamp=self.timestamp.value,
+            last_price=self.last_price.value,
+            bid_price=self.bid_price.value,
+            bid_volume=self.bid_volume.value,
+            ask_price=self.ask_price.value,
+            ask_volume=self.ask_volume.value,
+            order_book=None,
+            total_traded_volume=self.total_traded_volume.value,
+            total_traded_notional=self.total_traded_notional.value,
+            total_trade_count=self.total_trade_count.value,
         )
 
-        return self
+        return tick_data
 
-    @property
-    def market_time(self):
-        return datetime.datetime.fromtimestamp(self.timestamp)
 
-    @property
-    def market_price(self) -> float:
-        return np.nan
+class TransactionDataBuffer(_MarketDataMemoryBuffer):
+    def __init__(self):
+        super().__init__()
+
+        self.dtype = RawArray(c_wchar, 16)
+        self.price = RawValue(c_double)
+        self.volume = RawValue(c_double)
+        self.side = RawValue(c_int)
+
+        self.multiplier = RawValue(c_double)
+        self.notional = RawValue(c_double)
+        self.id_map = dict(
+            transaction_id=(RawValue(c_longlong), RawArray(c_wchar, 64)),  # id can be a int, str or None
+            buy_id=(RawValue(c_longlong), RawArray(c_wchar, 64)),
+            sell_id=(RawValue(c_longlong), RawArray(c_wchar, 64)),
+        )
 
+    def update(self, market_data: TradeData | TransactionData):
+        super().update(market_data=market_data)
 
-def get_data_attr(
-        data: list[MarketData] | dict[str, dict[datetime.datetime | datetime.date, MarketData] | list[MarketData]] = None,
-        key: str = 'close_price',
-        **kwargs
-) -> pd.DataFrame | pd.Series:
-    """
-    convert a dict[symbol, List[MarketData] or dict[symbol, MarketData]] dictionary to pandas data frame by a certain key(name)
-    :param data: dict of list of input MarketData
-    :param key: the key(name) to extract from
-    :return: a pandas DataFrame or pandas Series
-    """
-    historical_data = kwargs.pop('historical_data', None)
-    if historical_data is not None:
-        LOGGER.warning(DeprecationWarning('arg [historical_data] deprecated, use arg [data] instead'))
-        data = historical_data
-
-    data_dict = defaultdict(dict)
-
-    if isinstance(data, dict):
-        for ticker in data.keys():
-            if isinstance(data[ticker], dict):
-                market_data_list = data[ticker].values()
-            elif isinstance(data[ticker], Iterable):
-                market_data_list = data[ticker]
+        self.price.value = market_data['price']
+        self.volume.value = market_data['volume']
+        self.side.value = market_data['side']
+
+        if 'multiplier' in market_data:
+            self.multiplier.value = market_data['multiplier']
+        else:
+            self.multiplier.value = math.nan
+
+        if 'notional' in market_data:
+            self.multiplier.value = market_data['notional']
+        else:
+            self.multiplier.value = math.nan
+
+        for id_name in ['transaction_id', 'buy_id', 'sell_id']:
+            if id_name in market_data:
+                id_value = market_data[id_name]
+                if isinstance(id_value, int):
+                    self.id_map[id_name][0].value = id_value
+                    self.id_map[id_name][1].value = ''
+                elif isinstance(id_value, str):
+                    self.id_map[id_name][0].value = -1
+                    self.id_map[id_name][1].value = id_value
+                else:
+                    raise TypeError(f'Invalid {id_name} type: {type(id_name)}, expect int or str.')
             else:
-                raise TypeError(f'Invalid data Type {type(data[ticker])}')
-
-            for market_data in market_data_list:
-                data_dict[market_data.ticker][market_data.market_time] = getattr(market_data, key, float('nan'))
-    elif isinstance(data, Iterable):
-        for market_data in data:
-            data_dict[market_data.ticker][market_data.market_time] = getattr(market_data, key, float('nan'))
-    else:
-        raise TypeError(f'Invalid data Type {type(data)}')
+                self.id_map[id_name][0].value = -1
+                self.id_map[id_name][1].value = ''
 
-    result = pd.DataFrame(data_dict).sort_index(ascending=True)
+    def to_market_data(self) -> TradeData | TransactionData:
+        if math.isnan(multiplier := self.multiplier.value):
+            multiplier = None
 
-    if len(result.columns) == 1:
-        return result.iloc[:, 0]
-    else:
-        return result
+        if math.isnan(notional := self.multiplier.value):
+            notional = None
 
+        id_map = {}
+        for id_name in ['transaction_id', 'buy_id', 'sell_id']:
+            id_int = self.id_map[id_name][0].value
+            id_str = self.id_map[id_name][1].value
 
-def data_alignment(*args, **kwargs):
-    return get_data_attr(*args, **kwargs)
-
-
-def convert_to_bar(
-        data_sequence: dict[datetime.datetime, MarketData] | list[MarketData],
-        **kwargs,
-) -> dict[datetime.datetime, BarData]:
-    """
-    Convert tick / trade / bar data list or dict to bar data with given interval
-    :param data_sequence: dictionary or list of market data, DO NOT PASS A NEST DICT
-    :keyword bar_span: bar_span in timedelta, fallback to interval if not given
-    :keyword interval: bar_span in seconds, default = 60
-    :keyword trading_hour_checker: a check function return whether the given datetime is in trading hour. Use CN-A stock trading hour by default
-    :return: a dictionary with key = bar start time, value = minute bar data
-    """
-
-    if isinstance(data_sequence, dict):
-        market_data_list = list(data_sequence.values())
-    elif isinstance(data_sequence, list):
-        market_data_list = data_sequence
-    else:
-        raise Exception('Invalid data type')
-
-    if 'trading_hour_checker' not in kwargs:
-        def default_checker(mt):
-            if mt.time() < datetime.time(hour=9, minute=30) \
-                    or datetime.time(hour=11, minute=30) <= mt.time() < datetime.time(hour=13, minute=00) \
-                    or mt.time() >= datetime.time(hour=15, minute=00):
-                return False
+            if id_int == -1 and not id_str:
+                id_value = None
+            elif not id_str:
+                id_value = id_int
+            elif id_int == -1:
+                id_value = id_str
             else:
-                return True
+                raise ValueError(f'id_map can not contain both info of id_int={id_int}, id_str={id_str}.')
 
-        trading_hour_checker = default_checker
-    else:
-        trading_hour_checker = kwargs['trading_hour_checker']
-
-    bar_data_dict = {}
-
-    market_data_list.sort(key=lambda x: x.market_time)
-    last_tick_total_volume = 0.0
-    last_tick_total_notional = 0.0
-    last_tick_total_trades = 0
-
-    if 'bar_span' in kwargs:
-        bar_span = kwargs['bar_span']
-    else:
-        bar_span = datetime.timedelta(seconds=kwargs.get('interval', 60))
-
-    last_bar_start_time = None
-
-    bar_data = None
-    for market_data in market_data_list:  # type: MarketData
-        # if market data is not in active hours
-        if trading_hour_checker is not None and not trading_hour_checker(market_data.market_time):
-            if isinstance(market_data, TickData):
-                last_tick_total_volume = market_data.total_traded_volume
-                last_tick_total_notional = market_data.total_traded_notional
-                last_tick_total_trades = market_data.total_trade_count
-
-            continue
-        # with active bar data
-        if bar_data is not None:
-            # next trading day
-            if market_data.market_time.date() > bar_data.bar_start_time.date():
-                last_tick_total_volume = 0.0
-                last_tick_total_notional = 0.0
-                last_tick_total_trades = 0
-                last_bar_start_time = None
-                bar_data_dict[bar_data.bar_start_time] = bar_data
-            # next bar
-            if market_data.market_time > bar_data.bar_start_time + bar_span:
-                last_bar_start_time = bar_data.bar_start_time
-                bar_data_dict[bar_data.bar_start_time] = bar_data
-                bar_data = None
-            # current bar
-            else:
-                bar_data.high_price = max(bar_data.high_price, market_data.market_price)
-                bar_data.low_price = min(bar_data.low_price, market_data.market_price)
-                bar_data.close_price = market_data.market_price
-                if isinstance(market_data, TickData):
-                    bar_data.volume += market_data.total_traded_volume - last_tick_total_volume
-                    bar_data.notional += market_data.total_traded_notional - last_tick_total_notional
-                    bar_data.trade_count += market_data.total_trade_count - last_tick_total_trades
-
-                    last_tick_total_volume = market_data.total_traded_volume
-                    last_tick_total_notional = market_data.total_traded_notional
-                    last_tick_total_trades = market_data.total_trade_count
-                elif isinstance(market_data, TradeData):
-                    bar_data.volume += market_data.volume
-                    bar_data.notional += market_data.notional
-                    bar_data.trade_count += 1
-                elif isinstance(market_data, BarData):
-                    bar_data.volume += market_data.volume
-                    bar_data.notional += market_data.notional
-                    bar_data.trade_count += market_data.trade_count
-                else:
-                    pass
+            id_map[id_name] = id_value
 
-                if market_data.market_time == bar_data.bar_start_time + bar_span:
-                    last_bar_start_time = bar_data.bar_start_time
-                    bar_data_dict[bar_data.bar_start_time] = bar_data
-                    bar_data = None
-
-        if bar_data is None:
-            if last_bar_start_time is None:
-                bar_start_time = datetime.datetime(
-                    market_data.market_time.year,
-                    market_data.market_time.month,
-                    market_data.market_time.day,
-                    market_data.market_time.hour,
-                    market_data.market_time.minute
-                )
-            else:
-                i = (market_data.market_time - last_bar_start_time) // bar_span
-                bar_start_time = last_bar_start_time + i * bar_span
+        if (dtype := self.dtype.value) == 'TransactionData':
+            constructor = TransactionData
+        elif dtype == 'TradeData':
+            constructor = TradeData
+        else:
+            raise NotImplementedError(f'Constructor for market data {dtype} not implemented.')
 
-            bar_data = BarData(
-                ticker=market_data.ticker,
-                high_price=market_data.market_price,
-                low_price=market_data.market_price,
-                open_price=market_data.market_price,
-                close_price=market_data.market_price,
-                bar_start_time=bar_start_time,
-                bar_span=bar_span,
-            )
-
-            if isinstance(market_data, TickData):
-                bar_data.volume = market_data.total_traded_volume - last_tick_total_volume
-                bar_data.notional = market_data.total_traded_notional - last_tick_total_notional
-                bar_data.trade_count = market_data.total_trade_count - last_tick_total_trades
-
-                last_tick_total_volume = market_data.total_traded_volume
-                last_tick_total_notional = market_data.total_traded_notional
-                last_tick_total_trades = market_data.total_trade_count
-            elif isinstance(market_data, TradeData):
-                bar_data.volume = market_data.volume
-                bar_data.notional = market_data.notional
-                bar_data.trade_count = 1
-            elif isinstance(market_data, BarData):
-                bar_data.volume = market_data.volume
-                bar_data.notional = market_data.notional
-                bar_data.trade_count = market_data.trade_count
-            else:
-                pass
+        td = constructor(
+            ticker=self.ticker.value,
+            price=self.price.value,
+            volume=self.volume.value,
+            timestamp=self.timestamp.value,
+            side=self.side.value,
+            multiplier=multiplier,
+            notional=notional,
+            **id_map
+        )
 
-    return bar_data_dict
+        return td
```

### Comparing `pyquantkit-0.3.0/PyQuantKit/TradeUtils_old.py` & `pyquantkit-0.3.1/PyQuantKit/trade_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from __future__ import annotations
-
+import abc
 import copy
 import datetime
 import json
+import math
+import time
 import uuid
 from enum import Enum
+from typing import Self
 
-from . import LOGGER
+from . import LOGGER, TIME_ZONE
 from .market_utils import TransactionSide, TransactionData
 
 LOGGER = LOGGER.getChild('TradeUtils')
 __all__ = ['OrderState', 'OrderType', 'TradeInstruction', 'TradeReport']
 
 
 class OrderType(Enum):
@@ -66,501 +68,642 @@
                 self.value == OrderState.Rejected.value or \
                 self.value == OrderState.Invalid.value:
             return True
         else:
             return False
 
 
-class TradeReport(object):
+class TradeBaseClass(dict, metaclass=abc.ABCMeta):
+    def __init__(self, ticker: str, timestamp: float | None, **kwargs):
+        super().__init__(ticker=ticker, timestamp=timestamp)
+
+        if kwargs:
+            self['additional'] = dict(kwargs)
+
+    def __copy__(self):
+        return self.__class__.__init__(**self)
+
+    def copy(self):
+        return self.__copy__()
+
+    def to_json(self, fmt='str', **kwargs) -> str | dict:
+        data_dict = dict(
+            dtype=self.__class__.__name__,
+            **self
+        )
+
+        if 'additional' in data_dict:
+            additional = data_dict.pop('additional')
+            data_dict.update(additional)
+
+        if fmt == 'dict':
+            return data_dict
+        elif fmt == 'str':
+            return json.dumps(data_dict, **kwargs)
+        else:
+            raise ValueError(f'Invalid format {fmt}, except "dict" or "str".')
+
+    @classmethod
+    def from_json(cls, json_message: str | bytes | bytearray | dict) -> Self:
+        if isinstance(json_message, dict):
+            json_dict = json_message
+        else:
+            json_dict = json.loads(json_message)
+
+        dtype = json_dict.pop('dtype', None)
+        if dtype == 'TradeReport':
+            return TradeReport.from_json(json_dict)
+        elif dtype == 'TickData':
+            return TradeInstruction.from_json(json_dict)
+        else:
+            raise TypeError(f'Invalid dtype {dtype}')
+
+    @abc.abstractmethod
+    def to_list(self) -> list[float | int | str | bool]:
+        ...
+
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> Self:
+        dtype = data_list[0]
+
+        if dtype == 'TradeReport':
+            return TradeReport.from_list(data_list)
+        elif dtype == 'TradeInstruction':
+            return TradeInstruction.from_list(data_list)
+        else:
+            raise TypeError(f'Invalid dtype {dtype}')
+
+    @property
+    def ticker(self):
+        return self['ticker']
+
+    @property
+    def timestamp(self):
+        return self['timestamp']
+
+    @property
+    def additional(self):
+        if 'additional' not in self:
+            self['additional'] = {}
+        return self['additional']
+
+    @property
+    def topic(self) -> str:
+        return f'{self.ticker}.{self.__class__.__name__}'
+
+    @property
+    def market_time(self) -> datetime.datetime | datetime.date:
+        return datetime.datetime.fromtimestamp(self.timestamp, tz=TIME_ZONE)
+
+
+class TradeReport(TradeBaseClass):
+
     def __init__(
             self, *,
             ticker: str,
             side: int | float | str | TransactionSide,
+            price: float,
             volume: float,
-            notional: float,
+            timestamp: float,
             order_id: str,
-            timestamp: float = None,
-            trade_time: datetime.datetime = None,
-            price: float = None,
             trade_id: str = None,
-            multiplier: float = 1,
-            fee: float = .0
+            notional: float = None,
+            multiplier: float = None,
+            fee: float = None,
+            **kwargs
     ):
-        """
-        store trade report data
-        :param ticker: ticker (symbol) of the given asset (stock, future, option, crypto and etc.)
-        :param side: TransactionSide should be the same as TradeInstruction
-        :param volume: Traded volume (the number of shares, contracts or crypto, etc.)
-        :param notional: Traded notional (the amount of money) or premium of the option
-        :param timestamp: Timestamp when trade was matched
-        :param order_id: the id of its TradeInstruction
-        :param price: the traded price. NOTED: trade price does not necessarily equal notional / volume. For example, currency swap, crypto swap (future) and debt
-        :param trade_id: the id of itself
-        :param multiplier: multiplier for contract or option
-        :param fee: transition fee of this trade
-        """
         assert volume >= 0, 'Trade volume must not be negative'
+        assert notional >= 0, 'Trade notional must not be negative'
 
-        self.__ticker = str(ticker)
-        self.__side = TransactionSide(side)
-        self.__price = price
-        self.__volume = volume
-        self.__notional = notional
-        self.__timestamp = trade_time.timestamp() if timestamp is None else timestamp
-        self.__order_id = str(order_id)
-        self.__trade_id = str(trade_id) if trade_id is not None else str(uuid.uuid4())
-        self.__multiplier = float(multiplier)
-        self.__fee = fee
-
-    def __repr__(self):
-        return '<TradeReport>{}'.format({key: item.name if key == 'side' else item for key, item in self.__dict__.items()})
-
-    def __eq__(self, other):
-        if isinstance(other, TradeReport):
-            return self.__repr__() == other.__repr__()
-        else:
+        super().__init__(ticker=ticker, timestamp=timestamp, **kwargs)
+
+        self['price'] = price
+        self['volume'] = volume
+        self['side'] = int(side) if isinstance(side, (int, float)) else TransactionSide(side).value
+
+        self['order_id'] = order_id
+
+        if trade_id is not None:
+            self['trade_id'] = trade_id
+
+        if notional is not None and math.isfinite(notional):
+            self['notional'] = notional
+
+        if multiplier is not None and math.isfinite(multiplier):
+            self['multiplier'] = multiplier
+
+        if fee is not None and math.isfinite(fee):
+            self['fee'] = fee
+
+    def __eq__(self, other: Self):
+        assert isinstance(other, self.__class__), f'Can only compare with {self.__class__.__name__}'
+
+        # Fast check: only check the order id and trade id.
+        if not self.order_id == other.order_id:
             return False
+        elif not self.trade_id == other.trade_id:
+            return False
+
+        return True
 
     def __str__(self):
-        return f'<TradeReport>([{self.trade_time:%Y-%m-%d %H:%M:%S}] OrderID {self.order_id} {self.ticker} {self.side.name} {self.volume:.2f} @ {self.price:.2f} with trade_id {self.trade_id})'
+        return f'<TradeReport id={self.trade_id}>([{self.market_time:%Y-%m-%d %H:%M:%S}] {self.ticker} {TransactionSide(self.side).side_name} {self.volume} at {self.price})'
 
     def __reduce__(self):
         return self.__class__.from_json, (self.to_json(),)
 
-    def reset_order_id(self, order_id: str = None, **kwargs) -> TradeReport:
-        """
-        reset order_id id to given string
-        :param order_id: new order id, use UUID by default
-        :return:
-        """
-        if not kwargs.pop('_ignore_warning', False):
+    def reset_order_id(self, order_id: int | str = None, _ignore_warning: bool = False) -> Self:
+        if not _ignore_warning:
             LOGGER.warning('TradeReport OrderID being reset manually! TradeInstruction.reset_order_id() is the recommended method to do so.')
 
         if order_id is not None:
-            self.__order_id = str(order_id)
+            self['order_id'] = order_id
         else:
-            self.__order_id = str(uuid.uuid4())
+            self['order_id'] = uuid.uuid4().int
 
         return self
 
-    def reset_trade_id(self, trade_id: str = None) -> TradeReport:
-        """
-        reset trade id to given string
-        :param trade_id:
-        :return:
-        """
+    def reset_trade_id(self, trade_id: int | str = None) -> Self:
         if trade_id is not None:
-            self.__trade_id = str(trade_id)
+            self['trade_id'] = trade_id
         else:
-            self.__trade_id = str(uuid.uuid4())
+            self['trade_id'] = uuid.uuid4().int
 
         return self
 
     def to_trade(self) -> TransactionData:
         trade = TransactionData(
             ticker=self.ticker,
             timestamp=self.timestamp,
-            price=self.notional / self.volume / self.multiplier if self.volume > 0 else 0,
+            price=self.price,
             volume=self.volume,
             side=self.side,
             multiplier=self.multiplier
         )
         return trade
 
-    def to_json(self, fmt: str = 'str') -> str | dict:
-        json_dict = {
-            'ticker': self.__ticker,
-            'side': self.__side.name,
-            'price': self.__price,
-            'volume': self.__volume,
-            'notional': self.__notional,
-            'timestamp': self.__timestamp,
-            'order_id': self.__order_id,
-            'trade_id': self.__trade_id,
-            'multiplier': self.__multiplier,
-            'fee': self.__fee,
-        }
-
-        if fmt == 'dict':
-            return json_dict
-        else:
-            return json.dumps(json_dict)
+    def to_list(self) -> list[float | int | str | bool]:
+        return [self.__class__.__name__,
+                self.ticker,
+                self.timestamp,
+                self.price,
+                self.volume,
+                self['side'],
+                self.get('multiplier'),
+                self.get('notional'),
+                self.get('fee'),
+                self.get('trade_id'),
+                self.order_id]
 
     def copy(self, **kwargs):
         new_trade = self.__class__(
-            ticker=kwargs.pop('ticker', self.__ticker),
-            side=kwargs.pop('side', self.__side),
-            volume=kwargs.pop('volume', self.__volume),
-            notional=kwargs.pop('notional', self.__notional),
-            timestamp=kwargs.pop('timestamp', self.__timestamp),
-            order_id=kwargs.pop('order_id', None),
-            price=kwargs.pop('price', self.__price),
-            trade_id=kwargs.pop('trade_id', f'{self.__trade_id}.copy'),
-            multiplier=kwargs.pop('multiplier', self.__multiplier),
-            fee=kwargs.pop('fee', self.__fee)
+            ticker=kwargs.pop('ticker', self.ticker),
+            side=kwargs.pop('side', self.side),
+            price=kwargs.pop('price', self.price),
+            volume=kwargs.pop('volume', self.volume),
+            notional=kwargs.pop('notional', self.notional),
+            timestamp=kwargs.pop('timestamp', self.timestamp),
+            order_id=kwargs.pop('order_id', self.order_id),
+            trade_id=kwargs.pop('trade_id', f'{self.trade_id}.copy'),
+            multiplier=kwargs.pop('multiplier', self.multiplier),
+            fee=kwargs.pop('fee', self.fee)
         )
 
         return new_trade
 
     @classmethod
-    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TradeReport:
+    def from_json(cls, json_message: str | bytes | bytearray | dict) -> Self:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
-        self = cls(
-            ticker=json_dict['ticker'],
-            side=TransactionSide(json_dict['side']),
-            volume=json_dict['volume'],
-            price=json_dict['price'],
-            notional=json_dict['notional'],
-            timestamp=json_dict['timestamp'],
-            order_id=json_dict['order_id'],
-            trade_id=json_dict['trade_id'],
-            multiplier=json_dict['multiplier'],
-            fee=json_dict['fee'],
-        )
+        dtype = json_dict.pop('dtype', None)
+        if dtype is not None and dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
+        self = cls(**json_dict)
         return self
 
-    @staticmethod
-    def from_trade(trade_data: TradeData, order_id: str, trade_id: str = None) -> TradeReport:
-        report = TradeReport(
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> Self:
+        (dtype, ticker, timestamp, price, volume, side,
+         multiplier, notional, fee, trade_id, order_id) = data_list
+
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        kwargs = {}
+
+        if trade_id is not None:
+            kwargs['trade_id'] = trade_id
+
+        if notional is not None and math.isfinite(notional):
+            kwargs['notional'] = notional
+
+        if multiplier is not None and math.isfinite(multiplier):
+            kwargs['multiplier'] = multiplier
+
+        if fee is not None and math.isfinite(fee):
+            kwargs['fee'] = fee
+
+        return cls(
+            ticker=ticker,
+            timestamp=timestamp,
+            price=price,
+            volume=volume,
+            side=side,
+            order_id=order_id,
+            **kwargs
+        )
+
+    @classmethod
+    def from_trade(cls, trade_data: TransactionData, order_id: str, trade_id: str = None) -> Self:
+        report = cls(
             ticker=trade_data.ticker,
             side=trade_data.side,
             volume=trade_data.volume,
+            price=trade_data.price,
             notional=trade_data.notional,
             timestamp=trade_data.timestamp,
             order_id=order_id,
             trade_id=trade_id
         )
         return report
 
     @property
-    def multiplier(self) -> float:
-        return self.__multiplier
+    def price(self) -> float:
+        return self['price']
 
     @property
-    def fee(self) -> float:
-        return self.__fee
+    def volume(self) -> float:
+        return self['volume']
 
     @property
-    def ticker(self) -> str:
-        return self.__ticker
+    def side(self) -> TransactionSide:
+        return TransactionSide(self['side'])
 
     @property
-    def side(self) -> TransactionSide:
-        return self.__side
+    def multiplier(self) -> float:
+        return self.get('multiplier', 1.)
 
     @property
-    def volume(self) -> float:
-        return self.__volume
+    def fee(self) -> float:
+        return self.get('fee', 0.)
 
     @property
-    def notional(self) -> float:
-        return self.__notional
+    def order_id(self) -> int | str:
+        return self['order_id']
 
     @property
-    def price(self) -> float:
-        if self.__price is not None:
-            return self.__price
-        elif self.__volume == 0:
-            return .0
+    def trade_id(self) -> int | str:
+        if 'trade_id' in self:
+            trade_id = self['trade_id']
         else:
-            return self.__notional / self.__volume / self.__multiplier
+            trade_id = self['trade_id'] = uuid.uuid4().int
+
+        return trade_id
 
     @property
-    def trade_time(self) -> datetime.datetime:
-        return datetime.datetime.fromtimestamp(self.__timestamp)
+    def notional(self) -> float:
+        return self.get('notional', self.price * self.volume * self.multiplier)
 
     @property
-    def timestamp(self):
-        return self.__timestamp
+    def market_price(self) -> float:
+        return self.price
 
     @property
-    def order_id(self) -> str:
-        return self.__order_id
+    def flow(self):
+        return self.side.sign * self.volume
 
     @property
-    def trade_id(self) -> str:
-        return self.__trade_id
+    def trade_time(self) -> datetime.datetime:
+        return datetime.datetime.fromtimestamp(self.timestamp)
 
 
-class TradeInstruction(object):
+class TradeInstruction(TradeBaseClass):
     def __init__(
             self, *,
             ticker: str,
             side: int | float | str | TransactionSide,
-            order_type: OrderType = OrderType.Manual,
-            volume: float = 0.0,
+            volume: float,
+            timestamp: float,
+            order_type: int | float | str | OrderType = OrderType.Manual,
             limit_price: float = None,
             order_id: str = None,
-            multiplier: float = 1
+            multiplier: float = None,
+            **kwargs
     ):
-        if volume <= 0:
-            raise ValueError(f'Invalid trade volume {volume}!')
+        assert volume > 0, f'Invalid trade volume {volume}!'
+        super().__init__(ticker=ticker, timestamp=timestamp, **kwargs)
 
-        self.__ticker = str(ticker)
-        self.__side = TransactionSide(side)
-        self.__order_type = order_type
-        self.__volume = float(volume)
-        self.__limit_price = limit_price
-        self.__order_id = str(order_id) if order_id is not None else str(uuid.uuid4())
-        self.__multiplier = float(multiplier)
-
-        self.__order_state: OrderState = OrderState.Pending
-        self.__filled_volume: float = 0.0
-        self.__filled_notional: float = 0.0
-        self.__fee = .0
-        self.__start_datetime: datetime.datetime | None = None
-        self.__cancel_datetime: datetime.datetime | None = None
-        self.__finish_datetime: datetime.datetime | None = None
-        self.__trades: dict[str, TradeReport] = {}
-
-    def __repr__(self):
-        return '<TradeInstruction>{}'.format(self.__dict__)
-
-    def __eq__(self, other):
-        if isinstance(other, TradeInstruction):
-            return self.__repr__() == other.__repr__()
-        else:
+        self['volume'] = volume
+        self['side'] = int(side) if isinstance(side, (int, float)) else TransactionSide(side).value
+        self['order_type'] = int(order_type) if isinstance(order_type, (int, float)) else OrderType(order_type).value
+        self['order_id'] = order_id if order_id is not None else uuid.uuid4().int
+
+        if limit_price is not None and math.isfinite(limit_price):
+            self['limit_price'] = limit_price
+
+        if multiplier is not None and math.isfinite(multiplier):
+            self['multiplier'] = multiplier
+
+        self['order_state'] = OrderState.Pending.value
+        self['filled_volume'] = 0.
+        self['filled_notional'] = 0.
+        self['fee'] = 0.
+
+        # note that 3 additional entries might be added to the TradeInstruction
+        # self['ts_placed'] = timestamp
+        # self['ts_canceled'] = timestamp
+        # self['ts_finished'] = timestamp
+
+        self.trades: dict[int | str, TradeReport] = {}
+
+    def __eq__(self, other: Self):
+        assert isinstance(other, self.__class__), f'Can only compare with {self.__class__.__name__}'
+
+        # Fast check: only check the order id and trade id.
+        if not self.order_id == other.order_id:
             return False
 
+        return True
+
     def __str__(self):
         if self.limit_price is None or self.order_type == OrderType.MarketOrder:
-            return f'<TradeInstruction>({self.order_type.name} OrderID {self.order_id} {self.side.name} {self.ticker} {self.volume:.2f} filled {self.filled_volume:.2f} @ {self.average_price:.2f} now {self.order_state.name})'
+            return f'<TradeInstruction id={self.order_id}>({self.ticker} {self.order_type.name} {self.side.name} {self.volume}; filled {self.filled_volume:.2f} @ {self.average_price:.2f} now {self.order_state.name})'
         else:
-            return f'<TradeInstruction>({self.order_type.name} OrderID {self.order_id} {self.side.name} {self.ticker} {self.volume:.2f} limit {self.limit_price:.2f} filled {self.filled_volume:.2f} @ {self.average_price:.2f} now {self.order_state.name})'
+            return f'<TradeInstruction id={self.order_id}>({self.ticker} {self.order_type.name} {self.side.name} {self.volume} limit {self.limit_price:.2f}; filled {self.filled_volume:.2f} @ {self.average_price:.2f} now {self.order_state.name})'
 
     def __reduce__(self):
         return self.__class__.from_json, (self.to_json(),)
 
     def reset(self):
-        self.__trades = {}
+        self.trades.clear()
+        self.order_state = OrderState.Pending
 
-        self.__order_state: OrderState = OrderState.Pending
-        self.__filled_volume: float = 0.0
-        self.__filled_notional: float = 0.0
-        self.__fee = .0
-        self.__start_datetime: datetime.datetime | None = None
-        self.__cancel_datetime: datetime.datetime | None = None
-        self.__finish_datetime: datetime.datetime | None = None
-        self.__trades: dict[str, TradeReport] = {}
-
-    def reset_order_id(self, order_id: str = None, **kwargs) -> TradeInstruction:
-        """
-        reset order id to given string
-        :param order_id:
-        :return:
-        """
-        if not kwargs.pop('_ignore_warning', False):
-            LOGGER.warning('TradeInstruction OrderID being reset manually! Position.reset_order_id() is the recommended method to do so.')
+        self['filled_volume']: float = 0.0
+        self['filled_notional']: float = 0.0
+        self['fee'] = .0
+
+        self.pop('ts_placed', None)
+        self.pop('ts_canceled', None)
+        self.pop('ts_finished', None)
+
+    def reset_order_id(self, order_id: int | str = None, _ignore_warning: bool = False) -> Self:
+        if not _ignore_warning:
+            LOGGER.warning(f'{self.__class__.__name__} OrderID being reset manually! Position.reset_order_id() is the recommended method to do so.')
 
         if order_id is not None:
-            self.__order_id = str(order_id)
+            self['order_id'] = order_id
         else:
-            self.__order_id = str(uuid.uuid4())
+            self['order_id'] = uuid.uuid4().int
 
-        for trade_report in self.__trades.values():
-            trade_report.reset_order_id(order_id=self.__order_id, _ignore_warning=True)
+        for trade_report in self.trades.values():
+            trade_report.reset_order_id(order_id=self.order_id, _ignore_warning=True)
 
         return self
 
-    def set_order_state(self, order_state: OrderState, market_datetime: datetime.datetime = datetime.datetime.utcnow()) -> TradeInstruction:
-        self.__order_state = order_state
+    def set_order_state(self, order_state: OrderState, timestamp: float = time.time()) -> Self:
+        self.order_state = order_state
 
         # assign a start_datetime if order placed
         if order_state == OrderState.Placed:
-            self.__start_datetime = market_datetime
+            self['ts_placed'] = timestamp
+
+        elif order_state == OrderState.Filled:
+            self['ts_finished'] = timestamp
 
         if order_state == OrderState.Canceled:
-            self.__cancel_datetime = market_datetime
-            self.__finish_datetime = market_datetime
+            self['ts_canceled'] = timestamp
+            self['ts_finished'] = timestamp
 
         return self
 
-    def fill(self, trade_report: TradeReport) -> TradeInstruction:
+    def fill(self, trade_report: TradeReport) -> Self:
         if trade_report.order_id != self.order_id:
             LOGGER.warning(f'Order ID not match! Instruction ID {self.order_id}; Report ID {trade_report.order_id}')
             return self
 
         if trade_report.trade_id in self.trades:
-            LOGGER.warning('Duplicated trade received! Instruction {}; Report {}'.format(str(self), str(trade_report)))
+            LOGGER.warning(f'Duplicated trade received!\nInstruction {self}.\nReport {trade_report}.')
             return self
 
-        if trade_report.volume != 0:
+        if trade_report.volume:
             # update multiplier
-            if len(self.__trades) > 0:
-                assert self.__multiplier == trade_report.multiplier, 'Multiplier not match!'
-            else:
-                self.__multiplier = trade_report.multiplier
+            if 'multiplier' in trade_report:
+                if 'multiplier' not in self:
+                    self['multiplier'] = trade_report.multiplier
+                elif trade_report.multiplier != self['multiplier']:
+                    raise ValueError(f'Multiplier not match for order {self} and report {trade_report}.')
 
-            if trade_report.volume + self.__filled_volume > self.__volume:
-                LOGGER.warning('Fatal error!\nTradeInstruction: \n\t{}\nTradeReport:\n\t{}'.format(str(TradeInstruction), '\n\t'.join([str(x) for x in self.__trades.values()])))
+            if trade_report.volume + self.filled_volume > self.volume:
+                LOGGER.warning('Fatal error!\nTradeInstruction: \n\t{}\nTradeReport:\n\t{}'.format(str(TradeInstruction), '\n\t'.join([str(x) for x in self.trades.values()]) + f'\n\t<new> {trade_report}'))
                 raise ValueError('Fatal error! trade reports filled volume exceed order volume!')
 
-            self.__filled_volume += abs(trade_report.volume)
-            self.__filled_notional += abs(trade_report.notional)
+            self['filled_volume'] += abs(trade_report.volume)
+            self['filled_notional'] += abs(trade_report.notional)
 
-        if self.__filled_volume == self.__volume:
-            self.set_order_state(OrderState.Filled)
-            self.__finish_datetime = trade_report.trade_time
-        elif self.__filled_volume > 0:
-            self.set_order_state(OrderState.PartFilled)
+        if self.filled_volume == self.volume:
+            self.set_order_state(order_state=OrderState.Filled, timestamp=trade_report.timestamp)
+            self['ts_finished'] = trade_report.timestamp
+        elif self.filled_volume > 0:
+            self.set_order_state(order_state=OrderState.PartFilled)
 
-        self.__trades[trade_report.trade_id] = trade_report
+        self.trades[trade_report.trade_id] = trade_report
 
         return self
 
-    def cancel_order(self) -> TradeInstruction:
-        self.set_order_state(OrderState.Canceling)
+    def cancel_order(self) -> Self:
+        self.set_order_state(order_state=OrderState.Canceling)
 
         cancel_instruction = copy.copy(self)
-        cancel_instruction.__order_type = OrderType.CancelOrder
+        cancel_instruction.set_order_state(order_state=OrderState.Canceled)
 
         return cancel_instruction
 
-    def canceled(self, canceled_datetime: datetime.datetime) -> TradeInstruction:
+    def canceled(self, timestamp: float) -> Self:
         LOGGER.warning(DeprecationWarning('[canceled] depreciated! Use [set_order_state] instead!'), stacklevel=2)
 
-        self.set_order_state(OrderState.Canceled, canceled_datetime)
+        self.set_order_state(order_state=OrderState.Canceled, timestamp=timestamp)
         return self
 
     def to_json(self, with_trade=True, fmt: str = 'str') -> str | dict:
-        json_dict = {
-            'ticker': self.__ticker,
-            'side': self.__side.name,
-            'order_type': self.__order_type.name,
-            'volume': self.__volume,
-            'limit_price': self.__limit_price,
-            'order_id': self.__order_id,
-            'multiplier': self.__multiplier,
-            'order_state': self.__order_state.name,
-            'filled_volume': self.__filled_volume,
-            'filled_notional': self.__filled_notional,
-            'fee': self.__fee,
-            'start_datetime': None if self.__start_datetime is None else self.__start_datetime.timestamp(),
-            'cancel_datetime': None if self.__cancel_datetime is None else self.__cancel_datetime.timestamp(),
-            'finish_datetime': None if self.__finish_datetime is None else self.__finish_datetime.timestamp(),
-            'trades': {_: self.__trades[_].to_json(fmt='dict') for _ in self.__trades} if with_trade else {},
-        }
+        json_dict = super().to_json()
+
+        if self.trades:
+            json_dict['trade'] = [report.to_json(fmt='dict') for report in self.trades.values()]
 
         if fmt == 'dict':
             return json_dict
         else:
             return json.dumps(json_dict)
 
+    def to_list(self) -> list[float | int | str | bool]:
+        return [self.__class__.__name__,
+                self.ticker,
+                self.timestamp,
+                self.limit_price,
+                self.volume,
+                self['side'],
+                self['order_state'],
+                self.get('multiplier'),
+                self.get('notional'),
+                self.filled_volume,
+                self.filled_notional,
+                self.fee,
+                self.get('order_id')]
+
     @classmethod
-    def from_json(cls, json_message: str | bytes | bytearray | dict) -> TradeInstruction:
+    def from_json(cls, json_message: str | bytes | bytearray | dict) -> Self:
         if isinstance(json_message, dict):
             json_dict = json_message
         else:
             json_dict = json.loads(json_message)
 
-        self = cls(
-            ticker=json_dict['ticker'],
-            side=TransactionSide(json_dict['side']),
-            order_type=OrderType[json_dict['order_type']],
-            volume=json_dict['volume'],
-            limit_price=json_dict['limit_price'],
-            order_id=json_dict['order_id'],
-            multiplier=json_dict['multiplier']
-        )
+        dtype = json_dict.pop('dtype', None)
+        trades = json_dict.pop('trades', [])
 
-        self.__order_state = OrderState[json_dict['order_state']]
-        self.__filled_volume = json_dict['filled_volume']
-        self.__filled_notional = json_dict['filled_notional']
-        self.__fee = json_dict['fee']
-        self.__start_datetime = None if json_dict['start_datetime'] is None else datetime.datetime.fromtimestamp(json_dict['start_datetime'])
-        self.__cancel_datetime = None if json_dict['cancel_datetime'] is None else datetime.datetime.fromtimestamp(json_dict['cancel_datetime'])
-        self.__finish_datetime = None if json_dict['finish_datetime'] is None else datetime.datetime.fromtimestamp(json_dict['finish_datetime'])
+        if dtype is not None and dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
 
-        for trade_id in json_dict['trades']:
-            trade_json = json_dict['trades'][trade_id]
+        self = cls(**json_dict)
+
+        for trade_json in json_dict['trades']:
             report = TradeReport.from_json(trade_json)
-            self.__trades[report.trade_id] = report
+            self.trades[report.trade_id] = report
 
         return self
 
-    @property
-    def fee(self):
-        return self.__fee
+    @classmethod
+    def from_list(cls, data_list: list[float | int | str | bool]) -> Self:
+        (dtype, ticker, timestamp, limit_price, volume, side,
+         order_state, multiplier, notional, filled_volume, filled_notional, fee, order_id) = data_list
 
-    @fee.setter
-    def fee(self, value):
-        self.__fee = float(value)
+        if dtype != cls.__name__:
+            raise TypeError(f'dtype mismatch, expect {cls.__name__}, got {dtype}.')
+
+        kwargs = {}
+
+        if notional is not None and math.isfinite(notional):
+            kwargs['notional'] = notional
+
+        if multiplier is not None and math.isfinite(multiplier):
+            kwargs['multiplier'] = multiplier
+
+        if fee is not None and math.isfinite(fee):
+            kwargs['fee'] = fee
+
+        self = cls(
+            ticker=ticker,
+            timestamp=timestamp,
+            limit_price=limit_price,
+            volume=volume,
+            side=side,
+            order_id=order_id,
+            **kwargs
+        )
+
+        self['filled_volume'] = filled_volume
+        self['filled_notional'] = filled_notional
+        self['fee'] = fee
+
+        return self
 
     @property
     def is_working(self):
-        return self.__order_state.is_working
+        return self.order_state.is_working
 
     @property
     def is_done(self):
-        return self.__order_state.is_done
+        return self.order_state.is_done
 
     @property
-    def order_id(self) -> str:
-        return self.__order_id
+    def limit_price(self) -> float:
+        return self['limit_price']
 
     @property
-    def ticker(self) -> str:
-        return self.__ticker
+    def volume(self) -> float:
+        return self['volume']
 
     @property
     def side(self) -> TransactionSide:
-        return self.__side
+        return TransactionSide(self['side'])
 
     @property
-    def order_type(self) -> OrderType:
-        return self.__order_type
-
-    @property
-    def volume(self) -> float:
-        return self.__volume
+    def multiplier(self) -> float:
+        return self.get('multiplier', 1.)
 
     @property
-    def limit_price(self) -> float | None:
-        return self.__limit_price
+    def fee(self) -> float:
+        return self['fee']
 
-    @property
-    def start_time(self) -> datetime.datetime | None:
-        return self.__start_datetime
+    @fee.setter
+    def fee(self, value: float):
+        self['fee'] = value
 
     @property
-    def cancel_time(self) -> datetime.datetime | None:
-        return self.__cancel_datetime
+    def order_id(self) -> int | str:
+        return self['order_id']
 
     @property
-    def finish_time(self) -> datetime.datetime | None:
-        return self.__finish_datetime
+    def order_type(self) -> OrderType:
+        return OrderType(self['order_type'])
 
     @property
     def order_state(self) -> OrderState:
-        return self.__order_state
+        return OrderState(self['order_state'])
+
+    @order_state.setter
+    def order_state(self, value: OrderState):
+        if isinstance(value, int):
+            self['order_state'] = value
+        else:
+            self['order_state'] = OrderState(value).value
 
     @property
     def filled_volume(self) -> float:
-        return self.__filled_volume
+        return self['filled_volume']
 
     @property
     def working_volume(self) -> float:
-        return self.__volume - self.__filled_volume
+        return self.volume - self.filled_volume
 
     @property
     def filled_notional(self) -> float:
-        return self.__filled_notional
+        return self['filled_notional']
 
     @property
     def average_price(self) -> float:
-        if self.__filled_volume != 0:
-            return self.__filled_notional / self.__filled_volume / self.__multiplier
+        if self.filled_volume != 0:
+            return self.filled_notional / self.filled_volume / self.multiplier
         else:
             return float('NaN')
 
     @property
-    def trades(self) -> dict[str, TradeReport]:
-        return self.__trades
+    def start_time(self) -> datetime.datetime | None:
+        return datetime.datetime.fromtimestamp(self.timestamp, tz=TIME_ZONE)
 
     @property
-    def multiplier(self) -> float:
-        return self.__multiplier
+    def placed_time(self) -> datetime.datetime | None:
+        if 'placed_time' in self:
+            return datetime.datetime.fromtimestamp(self['placed_time'], tz=TIME_ZONE)
+
+        return None
+
+    @property
+    def canceled_time(self) -> datetime.datetime | None:
+        if 'ts_canceled' in self:
+            return datetime.datetime.fromtimestamp(self['ts_canceled'], tz=TIME_ZONE)
+
+        return None
+
+    @property
+    def finished_time(self) -> datetime.datetime | None:
+        if 'ts_finished' in self:
+            return datetime.datetime.fromtimestamp(self['ts_finished'], tz=TIME_ZONE)
+
+        return None
+
+
+class TradeOrder(TradeInstruction):
+    pass
```

### Comparing `pyquantkit-0.3.0/PyQuantKit/_FinanceDecimal.py` & `pyquantkit-0.3.1/PyQuantKit/_FinanceDecimal.py`

 * *Files identical despite different names*

### Comparing `pyquantkit-0.3.0/PyQuantKit/__init__.py` & `pyquantkit-0.3.1/PyQuantKit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 import logging
 import sys
 import time
 
 LOGGER: logging.Logger | None = None
 LOG_LEVEL = logging.INFO
```

### Comparing `pyquantkit-0.3.0/PyQuantKit/console_utils.py` & `pyquantkit-0.3.1/PyQuantKit/console_utils.py`

 * *Files identical despite different names*

### Comparing `pyquantkit-0.3.0/PyQuantKit/technical_analysis.py` & `pyquantkit-0.3.1/PyQuantKit/technical_analysis.py`

 * *Files identical despite different names*

### Comparing `pyquantkit-0.3.0/PyQuantKit.egg-info/PKG-INFO` & `pyquantkit-0.3.1/PyQuantKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQuantKit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Toolkit for Quantitative Finance
 Home-page: https://github.com/BolunHan/PyQuantKit.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyquantkit-0.3.0/setup.py` & `pyquantkit-0.3.1/setup.py`

 * *Files identical despite different names*

