# Comparing `tmp/uiautodev-0.3.7.tar.gz` & `tmp/uiautodev-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautodev-0.3.7.tar", max compression
+gzip compressed data, was "uiautodev-0.4.0.tar", max compression
```

## Comparing `uiautodev-0.3.7.tar` & `uiautodev-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2024-05-27 09:06:49.988979 uiautodev-0.3.7/LICENSE
--rw-r--r--   0        0        0     1191 2024-05-27 09:06:49.988979 uiautodev-0.3.7/README.md
--rw-r--r--   0        0        0     1144 2024-05-27 09:07:03.937050 uiautodev-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      267 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/__init__.py
--rw-r--r--   0        0        0      176 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/__main__.py
--rw-r--r--   0        0        0     2498 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/app.py
--rw-r--r--   0        0        0     1773 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/appium_proxy.py
--rw-r--r--   0        0        0     3919 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/case.py
--rw-r--r--   0        0        0     6234 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/cli.py
--rw-r--r--   0        0        0     4562 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/command_proxy.py
--rw-r--r--   0        0        0     1587 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/command_types.py
--rw-r--r--   0        0        0      552 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/common.py
--rw-r--r--   0        0        0     6827 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/android.py
--rw-r--r--   0        0        0     5308 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/appium.py
--rw-r--r--   0        0        0     2048 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/base_driver.py
--rw-r--r--   0        0        0     4353 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/ios.py
--rw-r--r--   0        0        0     2422 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/mock.py
--rw-r--r--   0        0        0  3675062 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
--rw-r--r--   0        0        0     8351 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/driver/udt/udt.py
--rw-r--r--   0        0        0      465 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/exceptions.py
--rw-r--r--   0        0        0      827 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/model.py
--rw-r--r--   0        0        0     2370 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/provider.py
--rw-r--r--   0        0        0     4425 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/router/device.py
--rw-r--r--   0        0        0      891 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/static/demo.html
--rw-r--r--   0        0        0     4785 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/common.py
--rw-r--r--   0        0        0      637 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/exceptions.py
--rw-r--r--   0        0        0    17386 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/usbmux.py
--rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 uiautodev-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-30 07:09:31.277629 uiautodev-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1191 2024-05-30 07:09:31.277629 uiautodev-0.4.0/README.md
+-rw-r--r--   0        0        0     1161 2024-05-30 07:09:43.385572 uiautodev-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-05-30 07:09:31.277629 uiautodev-0.4.0/uiautodev/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-30 07:09:31.277629 uiautodev-0.4.0/uiautodev/__main__.py
+-rw-r--r--   0        0        0     2498 2024-05-30 07:09:31.277629 uiautodev-0.4.0/uiautodev/app.py
+-rw-r--r--   0        0        0     1773 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/appium_proxy.py
+-rw-r--r--   0        0        0     3919 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/case.py
+-rw-r--r--   0        0        0     6234 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/cli.py
+-rw-r--r--   0        0        0     5007 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/command_proxy.py
+-rw-r--r--   0        0        0     1736 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/command_types.py
+-rw-r--r--   0        0        0      552 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/common.py
+-rw-r--r--   0        0        0     7207 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/driver/android.py
+-rw-r--r--   0        0        0     5308 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/driver/appium.py
+-rw-r--r--   0        0        0     2517 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/driver/base_driver.py
+-rw-r--r--   0        0        0     4238 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/driver/ios.py
+-rw-r--r--   0        0        0     2422 2024-05-30 07:09:31.281628 uiautodev-0.4.0/uiautodev/driver/mock.py
+-rw-r--r--   0        0        0  3675062 2024-05-30 07:09:31.289628 uiautodev-0.4.0/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
+-rw-r--r--   0        0        0     8351 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/driver/udt/udt.py
+-rw-r--r--   0        0        0      465 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/exceptions.py
+-rw-r--r--   0        0        0      827 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/model.py
+-rw-r--r--   0        0        0     2370 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/provider.py
+-rw-r--r--   0        0        0     4425 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/router/device.py
+-rw-r--r--   0        0        0      891 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/static/demo.html
+-rw-r--r--   0        0        0     4785 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/utils/common.py
+-rw-r--r--   0        0        0      637 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/utils/exceptions.py
+-rw-r--r--   0        0        0    17386 2024-05-30 07:09:31.293629 uiautodev-0.4.0/uiautodev/utils/usbmux.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 uiautodev-0.4.0/PKG-INFO
```

### Comparing `uiautodev-0.3.7/LICENSE` & `uiautodev-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/README.md` & `uiautodev-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/pyproject.toml` & `uiautodev-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "uiautodev"
-version = "0.3.7"
+version = "0.4.0"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pillow = "*"
-adbutils = "^2.6.0"
+adbutils = "^2.7.0"
 construct = "*"
 lxml = "*"
 click = "^8.1.7"
 pygments = ">=2"
 httpretty = {version = "^1.1.4", optional = true}
 appium-python-client = {version = "^4.0.0", optional = true}
 uiautomator2 = ">=2"
 httpx = "*"
 fastapi = "^0.111.0"
 uvicorn = {version = "*", extras = ["standard"]}
 poetry = "^1.8.2"
 pydantic = "^2.6"
+wdapy = "^0.2.2"
 
 [tool.poetry.extras]
 appium = ["appium-python-client", "httppretty"]
 
 [tool.poetry.scripts]
 "uiauto.dev" = "uiautodev.__main__:main"
 "uiautodev" = "uiautodev.__main__:main"
```

### Comparing `uiautodev-0.3.7/uiautodev/app.py` & `uiautodev-0.4.0/uiautodev/app.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/appium_proxy.py` & `uiautodev-0.4.0/uiautodev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/case.py` & `uiautodev-0.4.0/uiautodev/case.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/cli.py` & `uiautodev-0.4.0/uiautodev/cli.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/command_proxy.py` & `uiautodev-0.4.0/uiautodev/command_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,14 +101,39 @@
 
 
 @register(Command.HOME)
 def home(driver: BaseDriver):
     driver.home()
 
 
+@register(Command.BACK)
+def back(driver: BaseDriver):
+    driver.back()
+
+
+@register(Command.APP_SWITCH)
+def app_switch(driver: BaseDriver):
+    driver.app_switch()
+
+
+@register(Command.VOLUME_UP)
+def volume_up(driver: BaseDriver):
+    driver.volume_up()
+
+
+@register(Command.VOLUME_DOWN)
+def volume_down(driver: BaseDriver):
+    driver.volume_down()
+
+
+@register(Command.VOLUME_MUTE)
+def volume_mute(driver: BaseDriver):
+    driver.volume_mute()
+
+
 @register(Command.DUMP)
 def dump(driver: BaseDriver) -> DumpResponse:
     source, _ = driver.dump_hierarchy()
     return DumpResponse(value=source)
 
 
 @register(Command.WAKE_UP)
```

### Comparing `uiautodev-0.3.7/uiautodev/command_types.py` & `uiautodev-0.4.0/uiautodev/command_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,21 @@
     DUMP = "dump"
     WAKE_UP = "wakeUp"
     FIND_ELEMENTS = "findElements"
     CLICK_ELEMENT = "clickElement"
 
     LIST = "list"
 
+    # 0.4.0
+    BACK = "back"
+    APP_SWITCH = "appSwitch"
+    VOLUME_UP = "volumeUp"
+    VOLUME_DOWN = "volumeDown"
+    VOLUME_MUTE = "volumeMute"
+
 
 class TapRequest(BaseModel):
     x: Union[int, float]
     y: Union[int, float]
     isPercent: bool = False
```

### Comparing `uiautodev-0.3.7/uiautodev/common.py` & `uiautodev-0.4.0/uiautodev/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/driver/android.py` & `uiautodev-0.4.0/uiautodev/driver/android.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,14 +140,29 @@
         self.adb_device.app_stop(package)
 
     def home(self):
         self.adb_device.keyevent("HOME")
     
     def wake_up(self):
         self.adb_device.keyevent("WAKEUP")
+    
+    def back(self):
+        self.adb_device.keyevent("BACK")
+    
+    def app_switch(self):
+        self.adb_device.keyevent("APP_SWITCH")
+    
+    def volume_up(self):
+        self.adb_device.keyevent("VOLUME_UP")
+    
+    def volume_down(self):
+        self.adb_device.keyevent("VOLUME_DOWN")
+    
+    def volume_mute(self):
+        self.adb_device.keyevent("VOLUME_MUTE")
 
 
 def parse_xml(xml_data: str, wsize: WindowSize, display_id: Optional[int] = None) -> Node:
     root = ElementTree.fromstring(xml_data)
     node = parse_xml_element(root, wsize, display_id)
     if node is None:
         raise AndroidDriverException("Failed to parse xml")
```

### Comparing `uiautodev-0.3.7/uiautodev/driver/appium.py` & `uiautodev-0.4.0/uiautodev/driver/appium.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/driver/base_driver.py` & `uiautodev-0.4.0/uiautodev/driver/base_driver.py`

 * *Files 27% similar despite different names*

```diff
@@ -66,11 +66,31 @@
     def app_terminate(self, package: str):
         """ terminate app """
         raise NotImplementedError()
     
     def home(self):
         """ press home button """
         raise NotImplementedError()
+    
+    def back(self):
+        """ press back button """
+        raise NotImplementedError()
+
+    def app_switch(self):
+        """ switch app """
+        raise NotImplementedError()
+    
+    def volume_up(self):
+        """ volume up """
+        raise NotImplementedError()
+    
+    def volume_down(self):
+        """ volume down """
+        raise NotImplementedError()
+    
+    def volume_mute(self):
+        """ volume mute """
+        raise NotImplementedError()
 
     def wake_up(self):
         """ wake up the device """
         raise NotImplementedError()
```

### Comparing `uiautodev-0.3.7/uiautodev/driver/ios.py` & `uiautodev-0.4.0/uiautodev/driver/ios.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 import io
 import json
 import re
 from functools import partial
 from typing import List, Optional, Tuple
 from xml.etree import ElementTree
 
+import wdapy
 from PIL import Image
 
 from uiautodev.command_types import CurrentAppResponse
 from uiautodev.driver.base_driver import BaseDriver
 from uiautodev.exceptions import IOSDriverException
 from uiautodev.model import Node, WindowSize
-from uiautodev.utils.usbmux import MuxDevice, select_device
+from uiautodev.utils.usbmux import select_device
 
 
 class IOSDriver(BaseDriver):
     def __init__(self, serial: str):
         """ serial is the udid of the ios device """
         super().__init__(serial)
         self.device = select_device(serial)
+        self.wda = wdapy.AppiumUSBClient(self.device.serial)
     
     def _request(self, method: str, path: str, payload: Optional[dict] = None) -> bytes:
         conn = self.device.make_http_connection(port=8100)
         try:
             if payload is None:
                 conn.request(method, path)
             else:
@@ -52,37 +54,44 @@
     def _request_json_value(self, method: str, path: str) -> dict:
         return self._request_json(method, path)["value"]
     
     def status(self):
         return self._request_json("GET", "/status")
     
     def screenshot(self, id: int = 0) -> Image.Image:
-        png_base64 = self._request_json_value("GET", "/screenshot")
-        png_data = base64.b64decode(png_base64)
-        return Image.open(io.BytesIO(png_data))
+        return self.wda.screenshot()
     
     def window_size(self):
-        return self._request_json_value("GET", "/window/size")
+        return self.wda.window_size()
     
     def dump_hierarchy(self) -> Tuple[str, Node]:
         """returns xml string and hierarchy object"""
-        xml_data = self._request_json_value("GET", "/source")
+        t = self.wda.sourcetree()
+        xml_data = t.value
         root = ElementTree.fromstring(xml_data)
         return xml_data, parse_xml_element(root, WindowSize(width=1, height=1))
     
     def tap(self, x: int, y: int):
-        self._request("POST", f"/wda/tap/0", {"x": x, "y": y})
+        self.wda.tap(x, y)
     
     def app_current(self) -> CurrentAppResponse:
-        # {'processArguments': {'env': {}, 'args': []}, 'name': '', 'pid': 32, 'bundleId': 'com.apple.springboard'}
-        value = self._request_json_value("GET", "/wda/activeAppInfo")
-        return CurrentAppResponse(package=value["bundleId"], pid=value["pid"])
+        info = self.wda.app_current()
+        return CurrentAppResponse(package=info.bundle_id, pid=info.pid)
 
     def home(self):
-        self._request("POST", "/wda/homescreen")
+        self.wda.homescreen()
+    
+    def app_switch(self):
+        raise NotImplementedError()
+
+    def volume_up(self):
+        self.wda.volume_up()
+    
+    def volume_down(self):
+        self.wda.volume_down()
         
 
 def parse_xml_element(element, wsize: WindowSize, indexes: List[int]=[0]) -> Node:
     """
     Recursively parse an XML element into a dictionary format.
     # <XCUIElementTypeApplication type="XCUIElementTypeApplication" name="设置" label="设置" enabled="true" visible="true" accessible="false" x="0" y="0" width="414" height="896" index="0">
     """
```

### Comparing `uiautodev-0.3.7/uiautodev/driver/mock.py` & `uiautodev-0.4.0/uiautodev/driver/mock.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk` & `uiautodev-0.4.0/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/driver/udt/udt.py` & `uiautodev-0.4.0/uiautodev/driver/udt/udt.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/model.py` & `uiautodev-0.4.0/uiautodev/model.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/provider.py` & `uiautodev-0.4.0/uiautodev/provider.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/router/device.py` & `uiautodev-0.4.0/uiautodev/router/device.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/router/xml.py` & `uiautodev-0.4.0/uiautodev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/static/demo.html` & `uiautodev-0.4.0/uiautodev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/utils/common.py` & `uiautodev-0.4.0/uiautodev/utils/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/utils/exceptions.py` & `uiautodev-0.4.0/uiautodev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/uiautodev/utils/usbmux.py` & `uiautodev-0.4.0/uiautodev/utils/usbmux.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.7/PKG-INFO` & `uiautodev-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: uiautodev
-Version: 0.3.7
+Version: 0.4.0
 Summary: Mobile UI Automation, include UI hierarchy inspector, script recorder
 Home-page: https://uiauto.dev
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: appium
-Requires-Dist: adbutils (>=2.6.0,<3.0.0)
+Requires-Dist: adbutils (>=2.7.0,<3.0.0)
 Requires-Dist: appium-python-client (>=4.0.0,<5.0.0) ; extra == "appium"
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct
 Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: httpretty (>=1.1.4,<2.0.0)
 Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: pillow
 Requires-Dist: poetry (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic (>=2.6,<3.0)
 Requires-Dist: pygments (>=2)
 Requires-Dist: uiautomator2 (>=2)
 Requires-Dist: uvicorn[standard]
+Requires-Dist: wdapy (>=0.2.2,<0.3.0)
 Description-Content-Type: text/markdown
 
 # uiautodev
 [![codecov](https://codecov.io/gh/codeskyblue/appinspector/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/appinspector)
 [![PyPI version](https://badge.fury.io/py/uiautodev.svg)](https://badge.fury.io/py/uiautodev)
 
 https://uiauto.dev
```

