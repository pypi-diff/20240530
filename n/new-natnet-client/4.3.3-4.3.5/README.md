# Comparing `tmp/new_natnet_client-4.3.3.tar.gz` & `tmp/new_natnet_client-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.3.3.tar", max compression
+gzip compressed data, was "new_natnet_client-4.3.5.tar", max compression
```

## Comparing `new_natnet_client-4.3.3.tar` & `new_natnet_client-4.3.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.3/LICENSE
--rw-r--r--   0        0        0     1758 2024-05-16 01:55:55.789326 new_natnet_client-4.3.3/README.md
--rw-r--r--   0        0        0    16729 2024-05-29 17:18:42.013322 new_natnet_client-4.3.3/new_natnet_client/Client.py
--rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.3/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    25548 2024-05-16 02:29:37.345534 new_natnet_client-4.3.3/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.3/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      464 2024-05-29 17:19:36.306616 new_natnet_client-4.3.3/pyproject.toml
--rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 new_natnet_client-4.3.3/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.5/LICENSE
+-rw-r--r--   0        0        0     1758 2024-05-16 01:55:55.789326 new_natnet_client-4.3.5/README.md
+-rw-r--r--   0        0        0    16798 2024-05-29 21:59:58.708905 new_natnet_client-4.3.5/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.5/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    25548 2024-05-16 02:29:37.345534 new_natnet_client-4.3.5/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.5/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-29 22:00:37.758911 new_natnet_client-4.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 new_natnet_client-4.3.5/PKG-INFO
```

### Comparing `new_natnet_client-4.3.3/LICENSE` & `new_natnet_client-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.3/README.md` & `new_natnet_client-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.3/new_natnet_client/Client.py` & `new_natnet_client-4.3.5/new_natnet_client/Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from collections import deque
 import struct
 from types import NoneType, TracebackType
 from typing import Any, Optional, Tuple, Dict, Callable, Iterator, Type
 import socket
 import logging
 from threading import Thread, Lock
-from new_natnet_client.NatNetTypes import NAT_Messages, NAT_Data, MoCap, Descriptors
-from new_natnet_client.Unpackers import DataUnpackerV3_0, DataUnpackerV4_1
 from copy import copy, deepcopy
 import time
 
+from new_natnet_client.NatNetTypes import NAT_Messages, NAT_Data, MoCap, Descriptors
+from new_natnet_client.Unpackers import DataUnpackerV3_0, DataUnpackerV4_1
+
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 
 @dataclass(slots=True)
 class Server_info:
   application_name: str
   version: Tuple[int, ...]
   nat_net_major: int
@@ -26,15 +27,15 @@
   local_ip_address: str = "127.0.0.1"
   use_multicast: bool = True
   multicast_address: str ="239.255.42.99"
   command_port: int = 1510
   data_port: int = 1511
   max_buffer_size: InitVar[int] = 255
   __mocap_bytes: bytes | None = field(init=False, default=None)
-  __new_data_flag: bool = field(init=False, default=False)
+  __last_new_data_time: int = field(init=False, default=0)
   __descriptors: Descriptors = field(init=False, default_factory=Descriptors)
   __can_change_bitstream: bool = field(init=False, default=False)
   __running: bool = field(init=False, default=False)
   __command_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __data_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __freeze: bool = field(init=False, repr=False, default=False)
 
@@ -50,16 +51,19 @@
       return copy(self.__server_info)
 
   @property
   def MoCap(self) -> Iterator[MoCap]:
     if  self.__mocap_bytes is None: raise StopIteration
     while True:
       with self.__mocap_bytes_lock:
-        if self.__new_data_flag:
-          yield self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
+        yield self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
+  
+  @property
+  def last_new_data_time(self):
+    return self.__last_new_data_time  
 
   @property
   def server_responses(self) -> deque[int | str]:
     with self.__server_responses_lock:
       return self.__server_responses.copy()
 
   @property
@@ -251,16 +255,16 @@
     """
     self.__unpacker = DataUnpackerV3_0
     with self.__server_info_lock:
       if (self.__server_info.nat_net_major == 4 and self.__server_info.nat_net_minor >= 1) or self.__server_info.nat_net_major == 0:
         self.__unpacker = DataUnpackerV4_1
 
   def __unpack_mocap_data(self, data: bytes, packet_size: int) -> int:
+    self.__last_new_data_time = time.time_ns()
     with self.__mocap_bytes_lock:
-      self.__new_data_flag = True
       self.__mocap_bytes = data
     return packet_size
 
   def __unpack_data_descriptions(self, data: bytes, packet_size: int) -> int:
     offset = 0
     dataset_count = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     size_in_bytes = -1
```

### Comparing `new_natnet_client-4.3.3/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.3.5/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.3/new_natnet_client/Unpackers.py` & `new_natnet_client-4.3.5/new_natnet_client/Unpackers.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.3/PKG-INFO` & `new_natnet_client-4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.3.3
+Version: 4.3.5
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
```

