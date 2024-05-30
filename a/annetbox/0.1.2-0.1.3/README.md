# Comparing `tmp/annetbox-0.1.2.tar.gz` & `tmp/annetbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annetbox-0.1.2.tar", last modified: Thu May 23 16:56:11 2024, max compression
+gzip compressed data, was "annetbox-0.1.3.tar", last modified: Thu May 30 08:55:29 2024, max compression
```

## Comparing `annetbox-0.1.2.tar` & `annetbox-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1079 2024-05-22 15:57:41.000000 annetbox-0.1.2/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-23 16:56:11.450328 annetbox-0.1.2/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1320 2024-05-22 15:57:41.000000 annetbox-0.1.2/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1145 2024-05-23 16:55:56.000000 annetbox-0.1.2/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-05-23 16:56:11.450328 annetbox-0.1.2/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/annetbox/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 11:58:16.000000 annetbox-0.1.2/src/annetbox/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/annetbox/base/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:24:00.000000 annetbox-0.1.2/src/annetbox/base/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3633 2024-05-23 15:43:03.000000 annetbox-0.1.2/src/annetbox/base/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3992 2024-05-23 15:43:03.000000 annetbox-0.1.2/src/annetbox/base/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      312 2024-05-22 15:57:41.000000 annetbox-0.1.2/src/annetbox/base/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/annetbox/v24/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:46.000000 annetbox-0.1.2/src/annetbox/v24/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1471 2024-05-22 15:57:41.000000 annetbox-0.1.2/src/annetbox/v24/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1446 2024-05-22 15:57:41.000000 annetbox-0.1.2/src/annetbox/v24/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1346 2024-05-16 13:08:04.000000 annetbox-0.1.2/src/annetbox/v24/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/annetbox/v37/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:51.000000 annetbox-0.1.2/src/annetbox/v37/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3540 2024-05-23 16:55:47.000000 annetbox-0.1.2/src/annetbox/v37/client_async.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3426 2024-05-23 16:25:21.000000 annetbox-0.1.2/src/annetbox/v37/client_sync.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3442 2024-05-23 15:43:03.000000 annetbox-0.1.2/src/annetbox/v37/models.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-23 16:56:11.450328 annetbox-0.1.2/src/annetbox.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-23 16:56:11.000000 annetbox-0.1.2/src/annetbox.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      603 2024-05-23 16:56:11.000000 annetbox-0.1.2/src/annetbox.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-05-23 16:56:11.000000 annetbox-0.1.2/src/annetbox.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       92 2024-05-23 16:56:11.000000 annetbox-0.1.2/src/annetbox.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        9 2024-05-23 16:56:11.000000 annetbox-0.1.2/src/annetbox.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.560167 annetbox-0.1.3/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1079 2024-05-22 15:57:41.000000 annetbox-0.1.3/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-30 08:55:29.560167 annetbox-0.1.3/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1320 2024-05-22 15:57:41.000000 annetbox-0.1.3/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1145 2024-05-30 08:53:41.000000 annetbox-0.1.3/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-05-30 08:55:29.560167 annetbox-0.1.3/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.548167 annetbox-0.1.3/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.556167 annetbox-0.1.3/src/annetbox/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 11:58:16.000000 annetbox-0.1.3/src/annetbox/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.560167 annetbox-0.1.3/src/annetbox/base/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:24:00.000000 annetbox-0.1.3/src/annetbox/base/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3633 2024-05-23 15:43:03.000000 annetbox-0.1.3/src/annetbox/base/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3992 2024-05-23 15:43:03.000000 annetbox-0.1.3/src/annetbox/base/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      312 2024-05-22 15:57:41.000000 annetbox-0.1.3/src/annetbox/base/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.560167 annetbox-0.1.3/src/annetbox/v24/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:46.000000 annetbox-0.1.3/src/annetbox/v24/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1475 2024-05-30 08:52:13.000000 annetbox-0.1.3/src/annetbox/v24/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1449 2024-05-30 08:52:13.000000 annetbox-0.1.3/src/annetbox/v24/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1346 2024-05-16 13:08:04.000000 annetbox-0.1.3/src/annetbox/v24/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.560167 annetbox-0.1.3/src/annetbox/v37/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-05-16 12:00:51.000000 annetbox-0.1.3/src/annetbox/v37/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4026 2024-05-30 08:52:13.000000 annetbox-0.1.3/src/annetbox/v37/client_async.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3930 2024-05-30 08:52:13.000000 annetbox-0.1.3/src/annetbox/v37/client_sync.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3985 2024-05-30 08:52:13.000000 annetbox-0.1.3/src/annetbox/v37/models.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-05-30 08:55:29.560167 annetbox-0.1.3/src/annetbox.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)     2350 2024-05-30 08:55:29.000000 annetbox-0.1.3/src/annetbox.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      603 2024-05-30 08:55:29.000000 annetbox-0.1.3/src/annetbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-05-30 08:55:29.000000 annetbox-0.1.3/src/annetbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       92 2024-05-30 08:55:29.000000 annetbox-0.1.3/src/annetbox.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        9 2024-05-30 08:55:29.000000 annetbox-0.1.3/src/annetbox.egg-info/top_level.txt
```

### Comparing `annetbox-0.1.2/LICENSE` & `annetbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.2/PKG-INFO` & `annetbox-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annetbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annet Netbox client
 Author-email: Andrey Tikhonov <tishka17@nebius.com>
 License: MIT
 Project-URL: Source, https://github.com/annetutil/annetbox
 Project-URL: Homepage, https://github.com/annetutil/annetbox
 Project-URL: Bug Tracker, https://github.com/annetutil/annetbox/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `annetbox-0.1.2/README.md` & `annetbox-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.2/pyproject.toml` & `annetbox-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "annetbox"
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "tishka17@nebius.com" },
 ]
 license = { text = "MIT" }
 description = "Annet Netbox client"
 requires-python = ">=3.10"
```

### Comparing `annetbox-0.1.2/src/annetbox/base/client_async.py` & `annetbox-0.1.3/src/annetbox/base/client_async.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.2/src/annetbox/base/client_sync.py` & `annetbox-0.1.3/src/annetbox/base/client_sync.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.2/src/annetbox/v24/client_async.py` & `annetbox-0.1.3/src/annetbox/v24/client_sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from datetime import datetime
 
 import dateutil.parser
 from adaptix import Retort, loader
 from dataclass_rest import get
 
-from annetbox.base.client_async import BaseNetboxClient, collect
+from annetbox.base.client_sync import BaseNetboxClient, collect
 from annetbox.base.models import PagingResponse
 from .models import Device, Interface, IpAddress
 
 
 class NetboxV24(BaseNetboxClient):
     def _init_response_body_factory(self) -> Retort:
         return Retort(recipe=[loader(datetime, dateutil.parser.parse)])
 
     # dcim
-    @get("dcim/interfaces")
-    async def dcim_interfaces(
+    @get("dcim/interfaces/")
+    def dcim_interfaces(
         self,
         device_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Interface]:
         pass
 
     dcim_all_interfaces = collect(dcim_interfaces, field="device_id")
 
-    @get("dcim/devices")
-    async def dcim_devices(
+    @get("dcim/devices/")
+    def dcim_devices(
         self,
         name: list[str] | None = None,
         tag: str | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Device]:
         pass
 
     dcim_all_devices = collect(dcim_devices)
 
     @get("dcim/devices/{device_id}")
-    async def dcim_device(
+    def dcim_device(
         self,
         device_id: int,
     ) -> Device:
         pass
 
     # ipam
-    @get("ipam/ip-addresses")
-    async def ipam_ip_addresses(
+    @get("ipam/ip-addresses/")
+    def ipam_ip_addresses(
         self,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[IpAddress]:
         pass
```

### Comparing `annetbox-0.1.2/src/annetbox/v24/client_sync.py` & `annetbox-0.1.3/src/annetbox/v24/client_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from datetime import datetime
 
 import dateutil.parser
 from adaptix import Retort, loader
 from dataclass_rest import get
 
-from annetbox.base.client_sync import BaseNetboxClient, collect
+from annetbox.base.client_async import BaseNetboxClient, collect
 from annetbox.base.models import PagingResponse
 from .models import Device, Interface, IpAddress
 
 
 class NetboxV24(BaseNetboxClient):
     def _init_response_body_factory(self) -> Retort:
         return Retort(recipe=[loader(datetime, dateutil.parser.parse)])
 
     # dcim
-    @get("dcim/interfaces")
-    def dcim_interfaces(
+    @get("dcim/interfaces/")
+    async def dcim_interfaces(
         self,
         device_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Interface]:
         pass
 
     dcim_all_interfaces = collect(dcim_interfaces, field="device_id")
 
-    @get("dcim/devices")
-    def dcim_devices(
+    @get("dcim/devices/")
+    async def dcim_devices(
         self,
         name: list[str] | None = None,
         tag: str | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Device]:
         pass
 
     dcim_all_devices = collect(dcim_devices)
 
-    @get("dcim/devices/{device_id}")
-    def dcim_device(
+    @get("dcim/devices/{device_id}/")
+    async def dcim_device(
         self,
         device_id: int,
     ) -> Device:
         pass
 
     # ipam
-    @get("ipam/ip-addresses")
-    def ipam_ip_addresses(
+    @get("ipam/ip-addresses/")
+    async def ipam_ip_addresses(
         self,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[IpAddress]:
         pass
```

### Comparing `annetbox-0.1.2/src/annetbox/v24/models.py` & `annetbox-0.1.3/src/annetbox/v24/models.py`

 * *Files identical despite different names*

### Comparing `annetbox-0.1.2/src/annetbox/v37/client_async.py` & `annetbox-0.1.3/src/annetbox/v37/client_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .models import (
     Cable,
     Device,
     Interface,
     IpAddress,
     ItemToDelete,
     NewCable,
+    Prefix,
 )
 
 
 class NetboxV37(BaseNetboxClient):
     def _init_response_body_factory(self) -> FactoryProtocol:
         return Retort(recipe=[loader(datetime, dateutil.parser.parse)])
 
@@ -26,33 +27,35 @@
         return Retort(
             recipe=[
                 name_mapping(NewCable, omit_default=True),
             ],
         )
 
     # dcim
-    @get("dcim/interfaces")
+    @get("dcim/interfaces/")
     async def dcim_interfaces(
         self,
+        id: list[int] | None = None,
         device: list[str] | None = None,
         device__n: list[str] | None = None,
         device_id: list[int] | None = None,
         device_id__n: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Interface]:
         pass
 
     dcim_all_interfaces = collect(dcim_interfaces, field="device_id")
+    dcim_all_interfaces_by_id = collect(dcim_interfaces, field="id")
 
-    @get("dcim/interfaces/{id}")
+    @get("dcim/interfaces/{id}/")
     async def dcim_interface(self, id: int) -> Interface:
         pass
 
-    @get("dcim/cables")
+    @get("dcim/cables/")
     async def dcim_cables(
         self,
         device: list[str] | None = None,
         device_id: list[int] | None = None,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
@@ -63,64 +66,78 @@
 
     @post("dcim/cables/")
     async def dcim_cable_create(self, body: NewCable) -> Cable:
         pass
 
     @post("dcim/cables/")
     async def dcim_cable_bulk_create(
-            self, body: list[NewCable],
+        self,
+        body: list[NewCable],
     ) -> list[Cable]:
         pass
 
     @delete("dcim/cables/")
     async def _dcim_cable_bulk_delete(self, body: list[ItemToDelete]) -> None:
         pass
 
     async def dcim_cable_bulk_delete(self, body: Iterable[int]) -> None:
-        return await self._dcim_cable_bulk_delete([
-            ItemToDelete(id=x) for x in body
-        ])
+        return await self._dcim_cable_bulk_delete(
+            [ItemToDelete(id=x) for x in body],
+        )
 
-    @delete("dcim/cables/{id}")
+    @delete("dcim/cables/{id}/")
     async def dcim_cable_delete(self, id: int) -> None:
         pass
 
-    @get("dcim/devices")
+    @get("dcim/devices/")
     async def dcim_devices(
         self,
         name: list[str] | None = None,
         name__empty: bool | None = None,
         name__ic: list[str] | None = None,
         name__ie: list[str] | None = None,
         name__iew: list[str] | None = None,
         name__isw: list[str] | None = None,
         name__n: list[str] | None = None,
         name__nic: list[str] | None = None,
         name__nie: list[str] | None = None,
         name__niew: list[str] | None = None,
         name__nisw: list[str] | None = None,
+        id: list[int] | None = None,
         tag: list[str] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Device]:
         pass
 
     dcim_all_devices = collect(dcim_devices)
+    dcim_all_devices_by_id = collect(dcim_devices, field="id")
 
-    @get("dcim/devices/{device_id}")
+    @get("dcim/devices/{device_id}/")
     async def dcim_device(
         self,
         device_id: int,
     ) -> Device:
         pass
 
     # ipam
-    @get("ipam/ip-addresses")
+    @get("ipam/ip-addresses/")
     async def ipam_ip_addresses(
         self,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[IpAddress]:
         pass
 
     ipam_all_ip_addresses = collect(ipam_ip_addresses, field="interface_id")
+
+    @get("ipam/prefixes/")
+    def prefixes(
+        self,
+        prefix: list[str] | None = None,
+        limit: int = 20,
+        offset: int = 0,
+    ) -> PagingResponse[Prefix]:
+        pass
+
+    ipam_all_prefixes = collect(prefixes, field="prefix")
```

### Comparing `annetbox-0.1.2/src/annetbox/v37/client_sync.py` & `annetbox-0.1.3/src/annetbox/v37/client_sync.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .models import (
     Cable,
     Device,
     Interface,
     IpAddress,
     ItemToDelete,
     NewCable,
+    Prefix,
 )
 
 
 class NetboxV37(BaseNetboxClient):
     def _init_response_body_factory(self) -> FactoryProtocol:
         return Retort(recipe=[loader(datetime, dateutil.parser.parse)])
 
@@ -26,33 +27,35 @@
         return Retort(
             recipe=[
                 name_mapping(NewCable, omit_default=True),
             ],
         )
 
     # dcim
-    @get("dcim/interfaces")
+    @get("dcim/interfaces/")
     def dcim_interfaces(
         self,
+        id: list[int] | None = None,
         device: list[str] | None = None,
         device__n: list[str] | None = None,
         device_id: list[int] | None = None,
         device_id__n: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Interface]:
         pass
 
     dcim_all_interfaces = collect(dcim_interfaces, field="device_id")
+    dcim_all_interfaces_by_id = collect(dcim_interfaces, field="id")
 
-    @get("dcim/interfaces/{id}")
+    @get("dcim/interfaces/{id}/")
     def dcim_interface(self, id: int) -> Interface:
         pass
 
-    @get("dcim/cables")
+    @get("dcim/cables/")
     def dcim_cables(
         self,
         device: list[str] | None = None,
         device_id: list[int] | None = None,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
@@ -62,61 +65,77 @@
     dcim_all_cables = collect(dcim_cables, field="interface_id")
 
     @post("dcim/cables/")
     def dcim_cable_create(self, body: NewCable) -> Cable:
         pass
 
     @post("dcim/cables/")
-    def dcim_cable_bulk_create(self, body: list[NewCable]) -> list[Cable]:
+    def dcim_cable_bulk_create(
+        self,
+        body: list[NewCable],
+    ) -> list[Cable]:
         pass
 
     @delete("dcim/cables/")
     def _dcim_cable_bulk_delete(self, body: list[ItemToDelete]) -> None:
         pass
 
     def dcim_cable_bulk_delete(self, body: Iterable[int]) -> None:
         return self._dcim_cable_bulk_delete([ItemToDelete(id=x) for x in body])
 
-    @delete("dcim/cables/{id}")
+    @delete("dcim/cables/{id}/")
     def dcim_cable_delete(self, id: int) -> None:
         pass
 
-    @get("dcim/devices")
+    @get("dcim/devices/")
     def dcim_devices(
         self,
         name: list[str] | None = None,
         name__empty: bool | None = None,
         name__ic: list[str] | None = None,
         name__ie: list[str] | None = None,
         name__iew: list[str] | None = None,
         name__isw: list[str] | None = None,
         name__n: list[str] | None = None,
         name__nic: list[str] | None = None,
         name__nie: list[str] | None = None,
         name__niew: list[str] | None = None,
         name__nisw: list[str] | None = None,
+        id: list[int] | None = None,
         tag: list[str] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[Device]:
         pass
 
     dcim_all_devices = collect(dcim_devices)
+    dcim_all_devices_by_id = collect(dcim_devices, field="id")
 
-    @get("dcim/devices/{device_id}")
+    @get("dcim/devices/{device_id}/")
     def dcim_device(
         self,
         device_id: int,
     ) -> Device:
         pass
 
     # ipam
-    @get("ipam/ip-addresses")
+    @get("ipam/ip-addresses/")
     def ipam_ip_addresses(
         self,
         interface_id: list[int] | None = None,
         limit: int = 20,
         offset: int = 0,
     ) -> PagingResponse[IpAddress]:
         pass
 
     ipam_all_ip_addresses = collect(ipam_ip_addresses, field="interface_id")
+
+    @get("ipam/prefixes/")
+    def prefixes(
+        self,
+        prefix: list[str] | None = None,
+        limit: int = 20,
+        offset: int = 0,
+    ) -> PagingResponse[Prefix]:
+        pass
+
+    ipam_all_prefixes = collect(prefixes, field="prefix")
```

### Comparing `annetbox-0.1.2/src/annetbox/v37/models.py` & `annetbox-0.1.3/src/annetbox/v37/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,21 +44,35 @@
     id: int
     label: str
     display: str
     url: str
 
 
 @dataclass
+class InterfaceType:
+    value: str
+    label: str
+
+
+@dataclass
+class InterfaceConnectedEndpoint(Entity):
+    device: Entity
+
+
+@dataclass
 class Interface(Entity):
     cable: InterfaceCable | None
     cable_end: str
     device: Entity
     link_peers: list[LinkPeer]
     link_peers_type: str | None
     enabled: bool
+    type: InterfaceType
+    description: str
+    connected_endpoints: list[InterfaceConnectedEndpoint] | None
     created: datetime
     last_updated: datetime
 
 
 @dataclass
 class Device(Entity):
     url: str
@@ -173,7 +187,23 @@
     description: None | str = None
     comments: None | str = None
 
 
 @dataclass
 class ItemToDelete:
     id: int
+
+
+@dataclass
+class Prefix:
+    id: int
+    prefix: str
+    site: Entity | None
+    vrf: Entity | None
+    tenant: Entity | None
+    vlan: Entity | None
+    role: Entity | None
+    status: Label
+    is_pool: bool
+    custom_fields: dict[str, Any]
+    created: datetime
+    last_updated: datetime
```

### Comparing `annetbox-0.1.2/src/annetbox.egg-info/PKG-INFO` & `annetbox-0.1.3/src/annetbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annetbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annet Netbox client
 Author-email: Andrey Tikhonov <tishka17@nebius.com>
 License: MIT
 Project-URL: Source, https://github.com/annetutil/annetbox
 Project-URL: Homepage, https://github.com/annetutil/annetbox
 Project-URL: Bug Tracker, https://github.com/annetutil/annetbox/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `annetbox-0.1.2/src/annetbox.egg-info/SOURCES.txt` & `annetbox-0.1.3/src/annetbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

