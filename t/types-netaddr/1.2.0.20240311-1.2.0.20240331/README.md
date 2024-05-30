# Comparing `tmp/types-netaddr-1.2.0.20240311.tar.gz` & `tmp/types-netaddr-1.2.0.20240331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-netaddr-1.2.0.20240311.tar", last modified: Mon Mar 11 02:16:46 2024, max compression
+gzip compressed data, was "types-netaddr-1.2.0.20240331.tar", last modified: Sun Mar 31 02:18:30 2024, max compression
```

## Comparing `types-netaddr-1.2.0.20240311.tar` & `types-netaddr-1.2.0.20240331.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.477347 types-netaddr-1.2.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-11 02:16:45.000000 types-netaddr-1.2.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:16:45.000000 types-netaddr-1.2.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-11 02:16:46.477347 types-netaddr-1.2.0.20240311/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.473347 types-netaddr-1.2.0.20240311/netaddr-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 02:16:45.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.473347 types-netaddr-1.2.0.20240311/netaddr-stubs/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/contrib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/contrib/subnet_splitter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.473347 types-netaddr-1.2.0.20240311/netaddr-stubs/eui/
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/eui/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/eui/ieee.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/fbsocket.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.473347 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/iana.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/nmap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/rfc1924.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/ip/sets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.477347 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/eui48.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/eui64.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/ipv4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-11 02:14:35.000000 types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/ipv6.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:16:46.477347 types-netaddr-1.2.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-11 02:16:45.000000 types-netaddr-1.2.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:46.477347 types-netaddr-1.2.0.20240311/types_netaddr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-11 02:16:46.000000 types-netaddr-1.2.0.20240311/types_netaddr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-11 02:16:46.000000 types-netaddr-1.2.0.20240311/types_netaddr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:16:46.000000 types-netaddr-1.2.0.20240311/types_netaddr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-11 02:16:46.000000 types-netaddr-1.2.0.20240311/types_netaddr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.415418 types-netaddr-1.2.0.20240331/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-31 02:18:29.000000 types-netaddr-1.2.0.20240331/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:18:29.000000 types-netaddr-1.2.0.20240331/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-31 02:18:30.415418 types-netaddr-1.2.0.20240331/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.411418 types-netaddr-1.2.0.20240331/netaddr-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-31 02:18:29.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.411418 types-netaddr-1.2.0.20240331/netaddr-stubs/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/contrib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/contrib/subnet_splitter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.411418 types-netaddr-1.2.0.20240331/netaddr-stubs/eui/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/eui/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/eui/ieee.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/fbsocket.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.411418 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/iana.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/nmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/rfc1924.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/ip/sets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:29.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.415418 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/eui48.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/eui64.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/ipv4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-31 02:17:27.000000 types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/ipv6.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:30.415418 types-netaddr-1.2.0.20240331/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-31 02:18:29.000000 types-netaddr-1.2.0.20240331/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:30.415418 types-netaddr-1.2.0.20240331/types_netaddr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-31 02:18:30.000000 types-netaddr-1.2.0.20240331/types_netaddr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-31 02:18:30.000000 types-netaddr-1.2.0.20240331/types_netaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:30.000000 types-netaddr-1.2.0.20240331/types_netaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 02:18:30.000000 types-netaddr-1.2.0.20240331/types_netaddr.egg-info/top_level.txt
```

### Comparing `types-netaddr-1.2.0.20240311/CHANGELOG.md` & `types-netaddr-1.2.0.20240331/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.2.0.20240331 (2024-03-31)
+
+Remove bare Incomplete annotations in third-party stubs (#11671)
+
 ## 1.2.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
 
 ## 1.2.0.20240219 (2024-02-19)
 
 [stubsabot] Bump netaddr to 1.2.* (#11437)
```

### Comparing `types-netaddr-1.2.0.20240311/PKG-INFO` & `types-netaddr-1.2.0.20240331/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 1.2.0.20240311
+Version: 1.2.0.20240331
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-netaddr` aims to provide accurate annotations
 for `netaddr==1.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
```

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/__init__.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/core.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/core.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from _typeshed import Incomplete, SupportsWrite
+from _typeshed import SupportsWrite
 from collections.abc import Iterator, Mapping
 from typing import Final
 
 BIG_ENDIAN_PLATFORM: bool
 INET_PTON: Final = 1
 ZEROFILL: Final = 2
 NOHOST: Final = 4
 INET_ATON: Final = 8
 
 class AddrFormatError(Exception): ...
 class AddrConversionError(Exception): ...
 class NotRegisteredError(Exception): ...
 
 class Subscriber:
-    def update(self, data: Incomplete) -> None: ...
+    def update(self, data) -> None: ...
 
 class PrettyPrinter(Subscriber):
     fh: SupportsWrite[str]
     write_eol: bool
     def __init__(self, fh: SupportsWrite[str] = ..., write_eol: bool = True) -> None: ...
     def update(self, data: object) -> None: ...
```

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/eui/__init__.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/eui/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/eui/ieee.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/eui/ieee.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/ip/__init__.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/ip/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _typeshed import ConvertibleToInt, Incomplete, Unused
+from _typeshed import ConvertibleToInt, Unused
 from abc import abstractmethod
 from collections.abc import Iterable, Iterator
 from typing import Literal, SupportsIndex, SupportsInt, overload
 from typing_extensions import Self, TypeAlias
 
 from netaddr.core import DictDotLookup
 from netaddr.strategy.ipv6 import ipv6_verbose
@@ -88,15 +88,15 @@
     @overload
     def __getitem__(self, index: slice) -> Iterator[IPAddress]: ...
     @overload
     def __getitem__(self, index: SupportsIndex | slice) -> IPAddress | Iterator[IPAddress]: ...
     def __contains__(self, other: BaseIP | _IPAddressAddr) -> bool: ...
     def __bool__(self) -> Literal[True]: ...
 
-def parse_ip_network(module: Incomplete, addr: tuple[int, int] | str, flags: int = 0) -> tuple[int, int]: ...
+def parse_ip_network(module, addr: tuple[int, int] | str, flags: int = 0) -> tuple[int, int]: ...
 
 class IPNetwork(BaseIP, IPListMixin):
     def __init__(self, addr: _IPNetworkAddr, version: Literal[4, 6] | None = None, flags: int = 0) -> None: ...
     @property
     def prefixlen(self) -> int: ...
     @prefixlen.setter
     def prefixlen(self, value: int) -> None: ...
```

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/ip/glob.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/ip/glob.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/ip/iana.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/ip/iana.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def startElement(self, name: str, attrs: AttributesImpl) -> None: ...
     def endElement(self, name: str) -> None: ...
     def characters(self, content: str) -> None: ...
 
 class XMLRecordParser(Publisher):
     xmlparser: XMLReader
     fh: Incomplete
-    def __init__(self, fh: Incomplete, **kwargs: object) -> None: ...
+    def __init__(self, fh, **kwargs: object) -> None: ...
     def process_record(self, rec: Mapping[str, object]) -> dict[str, str] | None: ...
     def consume_record(self, rec: object) -> None: ...
     def parse(self) -> None: ...
     # Arbitrary attributes are set in __init__ with `self.__dict__.update(kwargs)`
     def __getattr__(self, name: str, /) -> Any: ...
 
 class IPv4Parser(XMLRecordParser):
@@ -41,12 +41,12 @@
     def normalise_addr(self, addr: str) -> str: ...
 
 class DictUpdater(Subscriber):
     dct: MutableMapping[_IanaInfoKey, Incomplete]
     topic: str
     unique_key: str
     def __init__(self, dct: MutableMapping[_IanaInfoKey, Incomplete], topic: str, unique_key: str) -> None: ...
-    def update(self, data: Incomplete) -> None: ...
+    def update(self, data) -> None: ...
 
 def load_info() -> None: ...
 def pprint_info(fh: SupportsWrite[str] | None = None) -> None: ...
 def query(ip_addr: IPAddress) -> dict[str, list[dict[str, str]]]: ...
```

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/ip/sets.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/ip/sets.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/__init__.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/eui48.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/eui48.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/eui64.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/eui64.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/ipv4.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/ipv4.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/netaddr-stubs/strategy/ipv6.pyi` & `types-netaddr-1.2.0.20240331/netaddr-stubs/strategy/ipv6.pyi`

 * *Files identical despite different names*

### Comparing `types-netaddr-1.2.0.20240311/setup.py` & `types-netaddr-1.2.0.20240331/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-netaddr` aims to provide accurate annotations
 for `netaddr==1.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.0.20240311",
+      version="1.2.0.20240331",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['netaddr-stubs'],
-      package_data={'netaddr-stubs': ['__init__.pyi', 'cli.pyi', 'compat.pyi', 'contrib/__init__.pyi', 'contrib/subnet_splitter.pyi', 'core.pyi', 'eui/__init__.pyi', 'eui/ieee.pyi', 'fbsocket.pyi', 'ip/__init__.pyi', 'ip/glob.pyi', 'ip/iana.pyi', 'ip/nmap.pyi', 'ip/rfc1924.pyi', 'ip/sets.pyi', 'strategy/__init__.pyi', 'strategy/eui48.pyi', 'strategy/eui64.pyi', 'strategy/ipv4.pyi', 'strategy/ipv6.pyi', 'METADATA.toml']},
+      package_data={'netaddr-stubs': ['__init__.pyi', 'cli.pyi', 'compat.pyi', 'contrib/__init__.pyi', 'contrib/subnet_splitter.pyi', 'core.pyi', 'eui/__init__.pyi', 'eui/ieee.pyi', 'fbsocket.pyi', 'ip/__init__.pyi', 'ip/glob.pyi', 'ip/iana.pyi', 'ip/nmap.pyi', 'ip/rfc1924.pyi', 'ip/sets.pyi', 'strategy/__init__.pyi', 'strategy/eui48.pyi', 'strategy/eui64.pyi', 'strategy/ipv4.pyi', 'strategy/ipv6.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-netaddr-1.2.0.20240311/types_netaddr.egg-info/PKG-INFO` & `types-netaddr-1.2.0.20240331/types_netaddr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-netaddr
-Version: 1.2.0.20240311
+Version: 1.2.0.20240331
 Summary: Typing stubs for netaddr
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/netaddr.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-netaddr` aims to provide accurate annotations
 for `netaddr==1.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/netaddr. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+with mypy 1.9.0, pyright 1.1.356, and
+pytype 2024.3.19.
```

### Comparing `types-netaddr-1.2.0.20240311/types_netaddr.egg-info/SOURCES.txt` & `types-netaddr-1.2.0.20240331/types_netaddr.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 netaddr-stubs/METADATA.toml
 netaddr-stubs/__init__.pyi
 netaddr-stubs/cli.pyi
 netaddr-stubs/compat.pyi
 netaddr-stubs/core.pyi
 netaddr-stubs/fbsocket.pyi
+netaddr-stubs/py.typed
 netaddr-stubs/contrib/__init__.pyi
 netaddr-stubs/contrib/subnet_splitter.pyi
 netaddr-stubs/eui/__init__.pyi
 netaddr-stubs/eui/ieee.pyi
 netaddr-stubs/ip/__init__.pyi
 netaddr-stubs/ip/glob.pyi
 netaddr-stubs/ip/iana.pyi
```

