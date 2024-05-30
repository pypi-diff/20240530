# Comparing `tmp/sniffing-io-0.1.1.tar.gz` & `tmp/sniffing_io-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffing-io-0.1.1.tar", last modified: Tue May 14 09:56:02 2024, max compression
+gzip compressed data, was "sniffing_io-0.2.0.tar", last modified: Thu May 30 18:41:29 2024, max compression
```

## Comparing `sniffing-io-0.1.1.tar` & `sniffing_io-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 09:56:02.101508 sniffing-io-0.1.1/
--rw-rw-rw-   0        0        0       44 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6214 2024-05-14 09:56:02.100508 sniffing-io-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing-io-0.1.1/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing-io-0.1.1/build.py
--rw-rw-rw-   0        0        0       13 2024-05-14 06:59:25.000000 sniffing-io-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 09:56:02.101508 sniffing-io-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1546 2024-05-14 09:55:59.000000 sniffing-io-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:56:02.099523 sniffing-io-0.1.1/sniffing_io.egg-info/
--rw-rw-rw-   0        0        0     6214 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/sniffing_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/sniffing_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/sniffing_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/sniffing_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 09:56:02.000000 sniffing-io-0.1.1/sniffing_io.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 09:56:02.098508 sniffing-io-0.1.1/sniffingio/
--rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing-io-0.1.1/sniffingio/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing-io-0.1.1/sniffingio/callbacks.py
--rw-rw-rw-   0        0        0      859 2024-03-07 07:55:55.000000 sniffing-io-0.1.1/sniffingio/data.py
--rw-rw-rw-   0        0        0     9571 2024-05-14 09:55:59.000000 sniffing-io-0.1.1/sniffingio/filters.py
--rw-rw-rw-   0        0        0     2490 2024-03-07 07:55:55.000000 sniffing-io-0.1.1/sniffingio/sniff.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/
+-rw-rw-rw-   0        0        0       44 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6214 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2024-03-07 09:00:19.000000 sniffing_io-0.2.0/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 sniffing_io-0.2.0/build.py
+-rw-rw-rw-   0        0        0       13 2024-05-14 06:59:25.000000 sniffing_io-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:41:29.891383 sniffing_io-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1546 2024-05-30 18:39:41.000000 sniffing_io-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.890382 sniffing_io-0.2.0/sniffing_io.egg-info/
+-rw-rw-rw-   0        0        0     6214 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 18:41:29.000000 sniffing_io-0.2.0/sniffing_io.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 18:41:29.889381 sniffing_io-0.2.0/sniffingio/
+-rw-rw-rw-   0        0        0      150 2024-03-02 10:06:09.000000 sniffing_io-0.2.0/sniffingio/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-03-04 08:50:47.000000 sniffing_io-0.2.0/sniffingio/callbacks.py
+-rw-rw-rw-   0        0        0      904 2024-05-30 18:24:06.000000 sniffing_io-0.2.0/sniffingio/data.py
+-rw-rw-rw-   0        0        0    10667 2024-05-30 18:28:33.000000 sniffing_io-0.2.0/sniffingio/filters.py
+-rw-rw-rw-   0        0        0     2514 2024-05-30 17:52:46.000000 sniffing_io-0.2.0/sniffingio/sniff.py
```

### Comparing `sniffing-io-0.1.1/PKG-INFO` & `sniffing_io-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.1.1/README.md` & `sniffing_io-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.1.1/build.py` & `sniffing_io-0.2.0/build.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.1.1/setup.py` & `sniffing_io-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sniffing-io',
-        version='0.1.1',
+        version='0.2.0',
         description=(
             "A simple package for packet sniffing, "
             "with static/dynamic filtering options, "
             "real-time reaction, I/O operations and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sniffing-io-0.1.1/sniffing_io.egg-info/PKG-INFO` & `sniffing_io-0.2.0/sniffing_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffing-io
-Version: 0.1.1
+Version: 0.2.0
 Summary: A simple package for packet sniffing, with static/dynamic filtering options, real-time reaction, I/O operations and more.
 Home-page: https://github.com/Shahaf-F-S/sniffing-io
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sniffing-io-0.1.1/sniffingio/callbacks.py` & `sniffing_io-0.2.0/sniffingio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sniffing-io-0.1.1/sniffingio/data.py` & `sniffing_io-0.2.0/sniffingio/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 from scapy.all import NetworkInterface, PacketList, Packet
 
 __all__ = [
     "SniffSettings",
     "NetworkInterface",
     "Packet",
-    "PacketList"
+    "PacketList",
+    "settings"
 ]
 
 @dataclass(slots=True)
 class SniffSettings:
 
     count: int = 0
     timeout: int = None
@@ -25,7 +26,9 @@
     callback: PacketCallback = None
     printer: bool | PacketCallback = None
     live_filter: LivePacketFilter = None
     stop_filter: LivePacketFilter = None
     interface: str | NetworkInterface = None
     static_filter: str | dict | PacketFilterOperand | Iterable[PacketFilterOperand] = None
     start_callback: Callable[[], ...] = None
+
+settings = SniffSettings
```

### Comparing `sniffing-io-0.1.1/sniffingio/filters.py` & `sniffing_io-0.2.0/sniffingio/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Iterable, Callable, ClassVar, Self
 from dataclasses import dataclass, asdict
 from abc import ABCMeta, abstractmethod
 
 from dacite import from_dict
 
-from scapy.all import Packet
+from scapy.all import Packet, sniff
 
 __all__ = [
     "PacketFilterOperand",
     "PacketFilter",
     "PacketFilterIntersection",
     "PacketFilterOperator",
     "PacketFilterUnion",
@@ -20,24 +20,43 @@
     "StaticPacketFilter",
     "BasePacketFilterOperator",
     "BasePacketFilterIntersection",
     "format_packet_filters",
     "LivePacketFilter",
     "dump_packet_filter",
     "load_packet_filter",
-    "PacketFilterValues"
+    "PacketFilterValues",
+    "Types",
+    "Names",
+    "pf",
+    "pfv"
 ]
 
 def wrap(value: str) -> str:
 
     if (" " in value) and not (value.startswith("(") and value.endswith(")")):
         value = f"({value})"
 
     return value
 
+class Names:
+
+    HOST = 'host'
+    PORT = 'port'
+    SRC = 'src'
+    DST = 'dst'
+
+class Types:
+
+    TCP = 'tcp'
+    UDP = 'udp'
+    ICMP = 'icmp'
+    SMTP = 'smtp'
+    MAC = 'mac'
+
 class BasePacketFilterOperator(metaclass=ABCMeta):
 
     @staticmethod
     def format_join(values: Iterable[str], joiner: str) -> str:
 
         if not values:
             return ""
@@ -133,49 +152,62 @@
 
         return from_dict(cls, data)
 
     def dump(self) -> dict[str, ...]:
 
         return asdict(self)
 
+    @abstractmethod
+    def match(self, packet: Packet) -> bool:
+
+        pass
+
 @dataclass(slots=True, frozen=True)
 class StaticPacketFilter(PacketFilterOperand):
 
     filter: str
 
     def format(self) -> str:
 
         return self.filter
 
+    def match(self, packet: Packet) -> bool:
+
+        return len(sniff(offline=packet, filter=self.filter, verbose=0)) > 0
+
 @dataclass(slots=True, frozen=True)
 class PacketFilterOperator(PacketFilterOperand, metaclass=ABCMeta):
 
-    filters: tuple["PacketFilterOperand", ...]
+    filters: tuple[PacketFilterOperand, ...]
 
     def __len__(self) -> int:
 
         return len(self.filters)
 
 @dataclass(slots=True, frozen=True)
 class PacketFilterUnion(PacketFilterOperator, BasePacketFilterUnion):
 
     def format(self) -> str:
 
-        return self.format_union(
-            (f.format() for f in self.filters or ())
-        )
+        return self.format_union((f.format() for f in self.filters or ()))
+
+    def match(self, packet: Packet) -> bool:
+
+        return any(f.match(packet) for f in self.filters)
 
 @dataclass(slots=True, frozen=True)
 class PacketFilterIntersection(PacketFilterOperator, BasePacketFilterIntersection):
 
     def format(self) -> str:
 
-        return self.format_intersection(
-            (f.format() for f in self.filters or ())
-        )
+        return self.format_intersection((f.format() for f in self.filters or ()))
+
+    def match(self, packet: Packet) -> bool:
+
+        return all(f.match(packet) for f in self.filters)
 
 @dataclass(slots=True, frozen=True)
 class PacketFilterNegation(PacketFilterOperand):
 
     filter: PacketFilterOperand
 
     ATTRIBUTES: ClassVar[set[str]] = {'filter'}
@@ -185,14 +217,18 @@
         data = self.filter.format()
 
         if not data:
             return ""
 
         return f"(not {data})"
 
+    def match(self, packet: Packet) -> bool:
+
+        return self.filter.match(packet)
+
 def layers_names(packet: Packet) -> list[str]:
 
     names = [packet.name]
 
     while packet.payload:
         packet = packet.payload
 
@@ -204,14 +240,15 @@
 class PacketFilterValues[T](PacketFilterOperand):
 
     types: list[str] = None
     names: list[str] = None
     values: list[T] = None
     source_values: list[T] = None
     destination_values: list[T] = None
+    attributes: dict[str, list[T]] = None
 
     @classmethod
     def load(cls, data: dict[str, list[T]]) -> "PacketFilterValues[T]":
 
         return from_dict(cls, data)
 
     def dump(self) -> dict[str, list[T]]:
@@ -258,65 +295,76 @@
             if values
         ]
 
         values = [value for value in values if value]
 
         return self.format_intersection(values)
 
-@dataclass(slots=True, frozen=True, eq=False)
-class PacketFilter(PacketFilterOperand):
-
-    data_link: PacketFilterValues[str] = None
-    internet: PacketFilterValues[str] = None
-    transportation: PacketFilterValues[int] = None
-
     def match(self, packet: Packet) -> bool:
 
-        layers = (self.data_link, self.internet, self.transportation)
-
-        for layer, layer_filter in zip(packet.layers(), layers):
-            if layer_filter is None:
-                continue
-
-            layer_filter: PacketFilterValues
+        for layer in packet.layers():
+            if (
+                (self.types is not None) and
+                (layer.name.lower() not in {n.lower() for n in self.types})
+            ):
+                return False
 
-            if layer.name.lower() not in {n.lower() for n in layer_filter.types}:
+            if (
+                self.attributes and
+                not all(
+                    hasattr(packet, attr) and
+                    getattr(packet, attr) in values
+                    for attr, values in self.attributes.items()
+                )
+            ):
                 return False
 
             if hasattr(layer, 'src'):
                 src = layer.src
                 dst = layer.dst
 
             elif hasattr(layer, 'sport'):
                 src = layer.sport
                 dst = layer.dport
 
             else:
                 continue
 
-            sources = layer_filter.values + layer_filter.source_values
-            destinations = layer_filter.values + layer_filter.destination_values
+            sources = (self.values or []) + (self.source_values or [])
+            destinations = (self.values or []) + (self.destination_values or [])
 
             if (
                 (sources and (src not in sources)) or
                 (destinations and (dst not in destinations))
             ):
                 return False
 
         return True
 
+@dataclass(slots=True, frozen=True, eq=False)
+class PacketFilter(PacketFilterOperand):
+
+    layers: list[PacketFilterValues] = None
+
+    def match(self, packet: Packet) -> bool:
+
+        for layer, layer_filter in zip(packet.layers(), self.layers):
+            if layer_filter is None:
+                continue
+
+            layer_filter: PacketFilterValues
+
+            if not layer_filter.match(layer):
+                return False
+
+        return True
+
     def format(self) -> str:
 
-        return self.format_intersection(
-            (
-                self.data_link.format(),
-                self.internet.format(),
-                self.transportation.format()
-            )
-        )
+        return self.format_intersection(layer.format() for layer in self.layers)
 
 def format_packet_filters(
         filters: BasePacketFilter | Iterable[BasePacketFilter],
         joiner: PacketFilterOperator = PacketFilterUnion
 ) -> str:
 
     if joiner is None:
@@ -372,7 +420,10 @@
     if isinstance(data, PacketFilterOperand):
         return data
 
     if isinstance(data, str):
         return StaticPacketFilter(data)
 
     return PacketFilterOperand.load(data)
+
+pfv = PacketFilterValues
+pf = PacketFilter
```

### Comparing `sniffing-io-0.1.1/sniffingio/sniff.py` & `sniffing_io-0.2.0/sniffingio/sniff.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,30 @@
     "Sniffer",
     "write_pcap",
     "read_pcap"
 ]
 
 class Sniffer:
 
-    def __init__(self, data: SniffSettings = None) -> None:
+    def __init__(self, settings: SniffSettings = None) -> None:
 
-        if data is None:
-            data = SniffSettings()
+        if settings is None:
+            settings = SniffSettings()
 
-        self.data = data
+        self.settings = settings
 
         self._sniffer = ScapyAsyncSniffer()
 
     def packets(self) -> PacketList:
 
         return cast(PacketList, self._sniffer.results)
 
     def start(self, data: SniffSettings = None) -> PacketList:
 
-        data = data or self.data or SniffSettings()
+        data = data or self.settings or SniffSettings()
 
         callback = None
 
         if data.callback and data.printer:
             callback = lambda p: (data.callback(p), data.printer(p))
 
         elif data.callback:
```

