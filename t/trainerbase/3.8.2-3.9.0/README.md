# Comparing `tmp/trainerbase-3.8.2.tar.gz` & `tmp/trainerbase-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainerbase-3.8.2.tar", max compression
+gzip compressed data, was "trainerbase-3.9.0.tar", max compression
```

## Comparing `trainerbase-3.8.2.tar` & `trainerbase-3.9.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1103 2024-01-06 22:32:03.489082 trainerbase-3.8.2/LICENSE
--rw-r--r--   0        0        0     1006 2024-02-07 20:32:53.128150 trainerbase-3.8.2/pyproject.toml
--rw-r--r--   0        0        0      611 2023-11-24 11:22:07.924711 trainerbase-3.8.2/README.rst
--rw-r--r--   0        0        0        0 2024-01-06 23:23:09.175674 trainerbase-3.8.2/trainerbase/__init__.py
--rw-r--r--   0        0        0     6101 2024-01-06 23:23:09.176788 trainerbase-3.8.2/trainerbase/codeinjection.py
--rw-r--r--   0        0        0       71 2024-01-06 23:23:09.179783 trainerbase-3.8.2/trainerbase/common/__init__.py
--rw-r--r--   0        0        0     3748 2024-02-07 20:30:04.436502 trainerbase-3.8.2/trainerbase/common/helpers.py
--rw-r--r--   0        0        0     3239 2024-01-07 01:52:04.666510 trainerbase-3.8.2/trainerbase/common/keyboard.py
--rw-r--r--   0        0        0     3921 2024-01-06 23:23:09.183780 trainerbase-3.8.2/trainerbase/common/teleport.py
--rw-r--r--   0        0        0      237 2024-01-06 23:23:09.184780 trainerbase-3.8.2/trainerbase/config.py
--rw-r--r--   0        0        0     5392 2024-01-06 23:23:09.185804 trainerbase-3.8.2/trainerbase/gameobject.py
--rw-r--r--   0        0        0      185 2024-01-06 23:23:09.187061 trainerbase-3.8.2/trainerbase/gui/__init__.py
--rw-r--r--   0        0        0     1275 2024-01-06 23:23:09.187061 trainerbase-3.8.2/trainerbase/gui/helpers.py
--rw-r--r--   0        0        0     1849 2024-01-06 23:23:09.188068 trainerbase-3.8.2/trainerbase/gui/injections.py
--rw-r--r--   0        0        0     1548 2024-02-07 20:32:59.345168 trainerbase-3.8.2/trainerbase/gui/misc.py
--rw-r--r--   0        0        0     5642 2024-02-07 20:32:59.409368 trainerbase-3.8.2/trainerbase/gui/objects.py
--rw-r--r--   0        0        0     1496 2024-01-06 23:23:09.190068 trainerbase-3.8.2/trainerbase/gui/scripts.py
--rw-r--r--   0        0        0     2900 2024-01-07 02:05:45.563132 trainerbase-3.8.2/trainerbase/gui/speedhack.py
--rw-r--r--   0        0        0     3113 2024-01-06 23:23:09.190576 trainerbase-3.8.2/trainerbase/gui/teleport.py
--rw-r--r--   0        0        0      136 2024-01-06 23:23:09.191584 trainerbase-3.8.2/trainerbase/gui/types.py
--rw-r--r--   0        0        0     1197 2024-01-06 23:23:09.192584 trainerbase-3.8.2/trainerbase/main.py
--rw-r--r--   0        0        0     4846 2024-01-06 23:23:09.192584 trainerbase-3.8.2/trainerbase/memory.py
--rw-r--r--   0        0        0     1920 2024-01-06 23:23:09.193584 trainerbase-3.8.2/trainerbase/scriptengine.py
--rw-r--r--   0        0        0     1608 2024-01-06 23:23:09.193584 trainerbase-3.8.2/trainerbase/speedhack.py
--rw-r--r--   0        0        0      626 2024-01-06 23:23:09.193584 trainerbase-3.8.2/trainerbase/tts.py
--rwxr-xr-x   0        0        0   117248 2023-11-24 11:22:07.934248 trainerbase-3.8.2/trainerbase_vendor/FASM.EXE
--rw-r--r--   0        0        0   349696 2023-11-29 19:52:21.040094 trainerbase-3.8.2/trainerbase_vendor/speedhack32.dll
--rw-r--r--   0        0        0   391168 2023-11-29 19:52:07.854801 trainerbase-3.8.2/trainerbase_vendor/speedhack64.dll
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 trainerbase-3.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-01-06 22:32:03.489082 trainerbase-3.9.0/LICENSE
+-rw-r--r--   0        0        0     1006 2024-02-09 19:32:19.701377 trainerbase-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0      611 2023-11-24 11:22:07.924711 trainerbase-3.9.0/README.rst
+-rw-r--r--   0        0        0        0 2024-02-08 19:21:34.796500 trainerbase-3.9.0/trainerbase/__init__.py
+-rw-r--r--   0        0        0     6101 2024-02-08 19:21:34.797531 trainerbase-3.9.0/trainerbase/codeinjection.py
+-rw-r--r--   0        0        0        0 2024-02-09 19:29:01.776059 trainerbase-3.9.0/trainerbase/common/__init__.py
+-rw-r--r--   0        0        0      343 2024-02-09 19:27:00.105112 trainerbase-3.9.0/trainerbase/common/abc.py
+-rw-r--r--   0        0        0     3748 2024-02-09 19:30:26.364652 trainerbase-3.9.0/trainerbase/common/helpers.py
+-rw-r--r--   0        0        0     3508 2024-02-09 19:32:26.952325 trainerbase-3.9.0/trainerbase/common/keyboard.py
+-rw-r--r--   0        0        0     3921 2024-02-08 19:21:34.799549 trainerbase-3.9.0/trainerbase/common/teleport.py
+-rw-r--r--   0        0        0      237 2024-02-08 19:21:34.800548 trainerbase-3.9.0/trainerbase/config.py
+-rw-r--r--   0        0        0     5678 2024-02-09 19:34:14.647762 trainerbase-3.9.0/trainerbase/gameobject.py
+-rw-r--r--   0        0        0      185 2024-02-08 19:21:34.801546 trainerbase-3.9.0/trainerbase/gui/__init__.py
+-rw-r--r--   0        0        0     1275 2024-02-08 19:21:34.802549 trainerbase-3.9.0/trainerbase/gui/helpers.py
+-rw-r--r--   0        0        0     1849 2024-02-08 19:21:34.803550 trainerbase-3.9.0/trainerbase/gui/injections.py
+-rw-r--r--   0        0        0     1896 2024-02-09 19:32:29.632364 trainerbase-3.9.0/trainerbase/gui/misc.py
+-rw-r--r--   0        0        0     5642 2024-02-09 19:32:29.755355 trainerbase-3.9.0/trainerbase/gui/objects.py
+-rw-r--r--   0        0        0     1496 2024-02-08 19:21:34.805544 trainerbase-3.9.0/trainerbase/gui/scripts.py
+-rw-r--r--   0        0        0     2900 2024-02-08 19:21:34.806545 trainerbase-3.9.0/trainerbase/gui/speedhack.py
+-rw-r--r--   0        0        0     3113 2024-02-08 19:21:34.807383 trainerbase-3.9.0/trainerbase/gui/teleport.py
+-rw-r--r--   0        0        0      136 2024-02-08 19:21:34.808396 trainerbase-3.9.0/trainerbase/gui/types.py
+-rw-r--r--   0        0        0     1197 2024-02-08 19:21:34.809532 trainerbase-3.9.0/trainerbase/main.py
+-rw-r--r--   0        0        0     4846 2024-02-08 19:21:34.810397 trainerbase-3.9.0/trainerbase/memory.py
+-rw-r--r--   0        0        0     1920 2024-02-08 19:21:34.810397 trainerbase-3.9.0/trainerbase/scriptengine.py
+-rw-r--r--   0        0        0     1608 2024-02-08 19:21:34.811395 trainerbase-3.9.0/trainerbase/speedhack.py
+-rw-r--r--   0        0        0      626 2024-02-08 19:21:34.812406 trainerbase-3.9.0/trainerbase/tts.py
+-rwxr-xr-x   0        0        0   117248 2023-11-24 11:22:07.934248 trainerbase-3.9.0/trainerbase_vendor/FASM.EXE
+-rw-r--r--   0        0        0   349696 2023-11-29 19:52:21.040094 trainerbase-3.9.0/trainerbase_vendor/speedhack32.dll
+-rw-r--r--   0        0        0   391168 2023-11-29 19:52:07.854801 trainerbase-3.9.0/trainerbase_vendor/speedhack64.dll
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 trainerbase-3.9.0/PKG-INFO
```

### Comparing `trainerbase-3.8.2/LICENSE` & `trainerbase-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/pyproject.toml` & `trainerbase-3.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trainerbase"
-version = "3.8.2"
+version = "3.9.0"
 description = "Framework for creating game trainers/mods"
 authors = ["v01d <v01d@v01d.ru>", "doomayka <zd@doomayka.ru>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/python-trainers/trainer-base"
 repository = "https://gitlab.com/python-trainers/trainer-base"
```

### Comparing `trainerbase-3.8.2/README.rst` & `trainerbase-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/codeinjection.py` & `trainerbase-3.9.0/trainerbase/codeinjection.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/common/helpers.py` & `trainerbase-3.9.0/trainerbase/common/helpers.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/common/keyboard.py` & `trainerbase-3.9.0/trainerbase/common/keyboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-from abc import ABC, abstractmethod
 from collections.abc import Callable
 from time import time
 from typing import override
 
 from keyboard import add_hotkey, on_press_key, on_release_key
 
-
-class Switchable(ABC):
-    @abstractmethod
-    def enable(self):
-        pass
-
-    @abstractmethod
-    def disable(self):
-        pass
+from trainerbase.common.abc import AbstractKeyboardHandler, Switchable
+from trainerbase.gameobject import GameBool
 
 
 class SimpleSwitchable(Switchable):
     def __init__(self, on_enabled: Callable[[], None], on_disabled: Callable[[], None]):
         self._on_enabled = on_enabled
         self._on_disabled = on_disabled
 
@@ -26,25 +18,14 @@
         self._on_enabled()
 
     @override
     def disable(self):
         self._on_disabled()
 
 
-class AbstractKeyboardHandler(ABC):
-    @property
-    @abstractmethod
-    def hotkey(self) -> str:
-        pass
-
-    @abstractmethod
-    def handle(self):
-        pass
-
-
 class SimpleHotkeyHandler(AbstractKeyboardHandler):
     def __init__(self, callback: Callable[[], None], hotkey: str):
         self._callback = callback
         self._hotkey = hotkey
 
     @property
     @override
@@ -72,14 +53,35 @@
 
     @property
     @override
     def hotkey(self):
         return self._key
 
     @override
+    def handle(self):
+        on_release_key(self._key, self._on_release)
+
+
+class GameBoolReleaseHotkeySwitch(AbstractKeyboardHandler):
+    def __init__(self, game_bool: GameBool, key: str):
+        self._key = key
+        self._game_bool = game_bool
+
+    def _on_release(self, _):
+        if self._game_bool.value:
+            self._game_bool.disable()
+        else:
+            self._game_bool.enable()
+
+    @property
+    @override
+    def hotkey(self):
+        return self._key
+
+    @override
     def handle(self):
         on_release_key(self._key, self._on_release)
 
 
 class ShortLongHotkeyPressSwitch(AbstractKeyboardHandler):
     def __init__(self, switchable: Switchable, key: str, short_press_max_delta: float = 0.3):
         self._key = key
```

### Comparing `trainerbase-3.8.2/trainerbase/common/teleport.py` & `trainerbase-3.9.0/trainerbase/common/teleport.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gameobject.py` & `trainerbase-3.9.0/trainerbase/gameobject.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Self, override
 
 from pymem.exception import MemoryWriteError
 
+from trainerbase.common.abc import Switchable
 from trainerbase.memory import ConvertibleToAddress, ensure_address, pm
 
 
 class AbstractReadableObject[T](ABC):
     @property
     @abstractmethod
     def value(self) -> T:
@@ -163,20 +164,28 @@
 class GameUnsignedLongLong(GameObject[int, int]):
     value_range: tuple[int, int] = (0, 18_446_744_073_709_551_615)
 
     pm_read = pm.read_ulonglong  # type: ignore
     pm_write = pm.write_ulonglong
 
 
-class GameBool(GameObject[bool, bool]):
+class GameBool(GameObject[bool, bool], Switchable):
     value_range: tuple[bool, bool] = (False, True)
 
     pm_read = pm.read_bool  # type: ignore
     pm_write = pm.write_bool
 
+    @override
+    def enable(self):
+        self.value = True  # pylint: disable=attribute-defined-outside-init
+
+    @override
+    def disable(self):
+        self.value = False  # pylint: disable=attribute-defined-outside-init
+
 
 class ReadonlyGameObjectSumGetter(AbstractReadableObject[int | float]):
     def __init__(self, *game_numbers: GameInt | GameFloat):
         self.game_numbers = game_numbers
 
     @property
     def value(self) -> int | float:
```

### Comparing `trainerbase-3.8.2/trainerbase/gui/helpers.py` & `trainerbase-3.9.0/trainerbase/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gui/injections.py` & `trainerbase-3.9.0/trainerbase/gui/injections.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gui/misc.py` & `trainerbase-3.9.0/trainerbase/gui/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,31 @@
 from dearpygui import dearpygui as dpg
 
 from trainerbase.common.keyboard import AbstractKeyboardHandler, ReleaseHotkeySwitch, ShortLongHotkeyPressSwitch
 from trainerbase.gui.types import AbstractUIComponent
 
 
 class SeparatorUI(AbstractUIComponent):
+    def __init__(self, empty_lines_before: int = 1, empty_lines_after: int = 0):
+        self._empty_lines_before = empty_lines_before
+        self._empty_lines_after = empty_lines_after
+
     @override
     def add_to_ui(self) -> None:
+        for _ in range(self._empty_lines_before):
+            dpg.add_text()
+
         dpg.add_separator()
 
+        for _ in range(self._empty_lines_after):
+            dpg.add_text()
+
 
 class TextUI(AbstractUIComponent):
-    def __init__(self, text: str):
+    def __init__(self, text: str = ""):
         self.text = text
 
     @override
     def add_to_ui(self) -> None:
         dpg.add_text(self.text)
```

### Comparing `trainerbase-3.8.2/trainerbase/gui/objects.py` & `trainerbase-3.9.0/trainerbase/gui/objects.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gui/scripts.py` & `trainerbase-3.9.0/trainerbase/gui/scripts.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gui/speedhack.py` & `trainerbase-3.9.0/trainerbase/gui/speedhack.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/gui/teleport.py` & `trainerbase-3.9.0/trainerbase/gui/teleport.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/main.py` & `trainerbase-3.9.0/trainerbase/main.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/memory.py` & `trainerbase-3.9.0/trainerbase/memory.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/scriptengine.py` & `trainerbase-3.9.0/trainerbase/scriptengine.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/speedhack.py` & `trainerbase-3.9.0/trainerbase/speedhack.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase/tts.py` & `trainerbase-3.9.0/trainerbase/tts.py`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase_vendor/FASM.EXE` & `trainerbase-3.9.0/trainerbase_vendor/FASM.EXE`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase_vendor/speedhack32.dll` & `trainerbase-3.9.0/trainerbase_vendor/speedhack32.dll`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/trainerbase_vendor/speedhack64.dll` & `trainerbase-3.9.0/trainerbase_vendor/speedhack64.dll`

 * *Files identical despite different names*

### Comparing `trainerbase-3.8.2/PKG-INFO` & `trainerbase-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainerbase
-Version: 3.8.2
+Version: 3.9.0
 Summary: Framework for creating game trainers/mods
 Home-page: https://gitlab.com/python-trainers/trainer-base
 License: MIT
 Author: v01d
 Author-email: v01d@v01d.ru
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

