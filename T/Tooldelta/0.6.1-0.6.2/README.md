# Comparing `tmp/tooldelta-0.6.1.tar.gz` & `tmp/tooldelta-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.6.1.tar", max compression
+gzip compressed data, was "tooldelta-0.6.2.tar", max compression
```

## Comparing `tooldelta-0.6.1.tar` & `tooldelta-0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1497 2024-05-19 08:25:37.225191 tooldelta-0.6.1/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-05-19 08:25:37.225191 tooldelta-0.6.1/README.md
--rw-r--r--   0        0        0      891 2024-05-19 08:25:50.897200 tooldelta-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0      618 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/auths.py
--rwxr-xr-x   0        0        0    12372 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10441 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/color_print.py
--rw-r--r--   0        0        0     1885 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/constants.py
--rwxr-xr-x   0        0        0    34764 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/frame.py
--rwxr-xr-x   0        0        0    13149 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    23814 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1832 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/logger.py
--rw-r--r--   0        0        0    29752 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1295 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/packets.py
--rwxr-xr-x   0        0        0    17541 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7821 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0    10499 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     6318 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/movent.py
--rw-r--r--   0        0        0     7025 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_load/utils.py
--rwxr-xr-x   0        0        0    17005 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16754 2024-05-19 08:25:37.229191 tooldelta-0.6.1/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1996 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/starter.py
--rwxr-xr-x   0        0        0     1110 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0    10039 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/urlmethod.py
--rw-r--r--   0        0        0    20711 2024-05-19 08:25:37.233191 tooldelta-0.6.1/tooldelta/utils.py
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 tooldelta-0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-05-30 11:53:36.472284 tooldelta-0.6.2/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-05-30 11:53:36.472284 tooldelta-0.6.2/README.md
+-rw-r--r--   0        0        0      908 2024-05-30 11:53:45.568294 tooldelta-0.6.2/pyproject.toml
+-rwxr-xr-x   0        0        0      618 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    12372 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10441 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1885 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/constants.py
+-rwxr-xr-x   0        0        0    35083 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/frame.py
+-rwxr-xr-x   0        0        0    13369 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    23814 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1832 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/logger.py
+-rw-r--r--   0        0        0    29752 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1295 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15701 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     9073 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0    10499 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     6318 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/movent.py
+-rw-r--r--   0        0        0     7025 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_load/utils.py
+-rwxr-xr-x   0        0        0    17005 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16754 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1996 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/starter.py
+-rwxr-xr-x   0        0        0     1110 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0    10039 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0    20711 2024-05-30 11:53:36.476284 tooldelta-0.6.2/tooldelta/utils.py
+-rw-r--r--   0        0        0     3624 1970-01-01 00:00:00.000000 tooldelta-0.6.2/PKG-INFO
```

### Comparing `tooldelta-0.6.1/LICENSE` & `tooldelta-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/README.md` & `tooldelta-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/pyproject.toml` & `tooldelta-0.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.6.1" # This field is automatically set to the value in the version file
+version = "0.6.2" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
 
 # Please don't change this manually, your changes may invalidate other people's package management, use poetry to make changes!
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 psutil = "5.9.8"
-requests = "2.31.0"
+requests = "2.32.0"
 ujson = "5.9.0"
 colorama = "^0.4.6"
 pillow = "^10.2.0"
 shellescape = "^3.8.1"
 pyspeedtest = "1.2.7"
 aiohttp = "^3.9.3"
 python-socketio = "5.11.1"
 flask = "^3.0.2"
 mido = "^1.3.2"
 websocket-client = "^1.7.0"
 fcwslib = "^3.0.0"
+pyyaml = "6.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tooldelta-0.6.1/tooldelta/__init__.py` & `tooldelta-0.6.2/tooldelta/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/auths.py` & `tooldelta-0.6.2/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/cfg.py` & `tooldelta-0.6.2/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/color_print.py` & `tooldelta-0.6.2/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/constants.py` & `tooldelta-0.6.2/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/frame.py` & `tooldelta-0.6.2/tooldelta/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,21 +525,21 @@
         """获取控制台命令列表
 
         Returns:
             list: 命令列表
         """
         return self.consoleMenu
 
-    def set_game_control(self, game_ctrl) -> None:
+    def set_game_control(self, game_ctrl: "GameCtrl") -> None:
         """使用外源GameControl
 
         Args:
             game_ctrl (_type_): GameControl对象
         """
-        self.link_game_ctrl: "GameCtrl" = game_ctrl
+        self.link_game_ctrl = game_ctrl
 
     def set_plugin_group(self, plug_grp) -> None:
         """使用外源PluginGroup
 
         Args:
             plug_grp (_type_): PluginGroup对象
         """
@@ -783,43 +783,46 @@
     def say_to(self, target: str, msg: str) -> None:
         """向玩家发送消息
 
         Args:
             target (str): 玩家名/目标选择器
             msg (str): 消息
         """
-        self.sendwocmd("tellraw " + target +
-                       ' {"rawtext":[{"text":"' + msg + '"}]}')
+        text_json = json.dumps({"rawtext": [{"text": msg}]}, ensure_ascii=False)
+        self.sendwocmd("tellraw " + target + text_json)
 
     def player_title(self, target: str, text: str) -> None:
         """向玩家展示标题文本
 
         Args:
             target (str): 玩家名/目标选择器
             text (str): 文本
         """
-        self.sendwocmd(f"title {target} title {text}")
+        text_json = json.dumps({"rawtext": [{"text": text}]}, ensure_ascii=False)
+        self.sendwocmd(f"titleraw " + target + " title " + text_json)
 
     def player_subtitle(self, target: str, text: str) -> None:
         """向玩家展示副标题文本
 
         Args:
             target (str): 玩家名/目标选择器
             text (str): 文本
         """
-        self.sendwocmd(f"title {target} subtitle {text}")
+        text_json = json.dumps({"rawtext": [{"text": text}]}, ensure_ascii=False)
+        self.sendwocmd(f"titleraw " + target + " subtitle " + text_json)
 
     def player_actionbar(self, target: str, text: str) -> None:
         """向玩家展示动作栏文本
 
         Args:
             target (str): 玩家名/目标选择器
             text (str): 文本
         """
-        self.sendwocmd(f"title {target} actionbar {text}")
+        text_json = json.dumps({"rawtext": [{"text": text}]}, ensure_ascii=False)
+        self.sendwocmd(f"titleraw " + target + " actionbar " + text_json)
 
     def get_game_data(self) -> dict:
         """获取游戏数据
 
         Returns:
             dict: 游戏数据
         """
```

### Comparing `tooldelta-0.6.1/tooldelta/game_texts.py` & `tooldelta-0.6.2/tooldelta/game_texts.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from glob import glob
 from typing import Dict
 import warnings
 import requests
 import ujson as json
 import urllib3
 from .urlmethod import download_file_singlethreaded
+from .get_tool_delta_version import get_tool_delta_version
 from .color_print import Print
 from .sys_args import sys_args_to_dict
 # 关闭警告
 urllib3.disable_warnings()
 warnings.filterwarnings("ignore")
 
 class GameTextsLoader:
@@ -33,14 +34,15 @@
     @staticmethod
     def get_latest_version() -> str:
         """获取最新版本号
 
         Returns:
             str: 版本号
         """
+        if "no-download-libs" in sys_args_to_dict().keys() or "no-update-check" in sys_args_to_dict().keys():return '.'.join(map(str, get_tool_delta_version()))
         result = re.match(
             r"(\d+\.\d+\.\d+)",
             requests.get(
                 "https://api.github.com/repos/ToolDelta/GameText/releases/latest", timeout=5, verify=True
             ).json()["tag_name"],
         )
         if not isinstance(result, type(None)):
```

### Comparing `tooldelta-0.6.1/tooldelta/launch_cli.py` & `tooldelta-0.6.2/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/launch_options.py` & `tooldelta-0.6.2/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/logger.py` & `tooldelta-0.6.2/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/neo_conn.py` & `tooldelta-0.6.2/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/packets.py` & `tooldelta-0.6.2/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.6.2/tooldelta/plugin_load/PluginGroup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 "插件加载器框架"
 import asyncio
 import traceback
 from typing import TYPE_CHECKING, Any, Callable, Union, TypeVar
 
-PLUGIN_CLS_TYPE = TypeVar("PLUGIN_CLS_TYPE")
-
 from ..color_print import Print
-from ..plugin_load.classic_plugin import Plugin
+from .classic_plugin import (
+    Plugin,
+    add_plugin,
+    add_plugin_as_api
+)
 from ..utils import Utils
 from .injected_plugin import (
     execute_init,
     execute_player_prejoin,
     execute_player_join,
     execute_player_message,
     execute_death_message,
@@ -29,29 +31,31 @@
 from ..constants import PRG_NAME
 from .utils import set_frame as _set_frame
 from .injected_plugin.movent import set_frame as _set_frame_inj
 
 if TYPE_CHECKING:
     from ..frame import Frame, GameCtrl
 
+_TV = TypeVar("_TV")
+_SUPER_CLS = TypeVar("_SUPER_CLS")
+
 class PluginGroup:
     "插件组"
-    plugins: list[list[str | Plugin]] = []
+    plugins: list[Plugin] = []
     plugins_funcs: dict[str, list] = {
         "on_def": [],
         "on_inject": [],
         "on_player_prejoin": [],
         "on_player_join": [],
         "on_player_message": [],
         "on_player_death": [],
         "on_player_leave": [],
         "on_frame_exit": []
     }
-    plugin_added_cache = {"plugin": None, "packets": []}
-    pluginAPI_added_cache = []
+    plugin_added_cache = {"packets": []}
     broadcast_evts_cache = {}
 
     def __init__(self):
         "初始化"
         self._listen_packet_ids = set()
         self._packet_funcs: dict[str, list[Callable]] = {}
         self._broadcast_listeners: dict[str, list[Callable]] = {}
@@ -59,94 +63,60 @@
         self.plugins_api: dict[str, Plugin] = {}
         self.excType = 0
         self.normal_plugin_loaded_num = 0
         self.injected_plugin_loaded_num = 0
         self.loaded_plugins_name = []
         self.linked_frame: Union["Frame" , None] = None
 
-    def add_plugin(self, plugin: type[PLUGIN_CLS_TYPE]) -> type[PLUGIN_CLS_TYPE]:
-        """添加插件
-
-        Args:
-            plugin (type[Plugin]): 插件主类
-
-        Raises:
-            NotValidPluginError: 插件主类必须继承Plugin类
-
-        Returns:
-            type[Plugin]: 插件主类
-        """
-        try:
-            if not Plugin.__subclasscheck__(plugin):
-                raise NotValidPluginError(f"插件主类必须继承Plugin类 而不是 {plugin}")
-        except TypeError as exc:
-            raise NotValidPluginError(
-                f"插件主类必须继承Plugin类 而不是 {plugin.__class__}") from exc
-        self.plugin_added_cache["plugin"] = plugin
-        self.test_plugin(plugin) # type: ignore
-        return plugin
-
-    def add_plugin_as_api(self, apiName: str):
-        """添加插件作为API
+    add_plugin = staticmethod(add_plugin)
 
-        Args:
-            apiName (str): API名
+    add_plugin_as_api = staticmethod(add_plugin_as_api)
 
-        Returns:
-            Callable[[type[Plugin]], type[Plugin]]: 添加插件作为API
+    def add_packet_listener(self, pktID: int | list[int]):
         """
-        def _add_plugin_2_api(api_plugin: type[PLUGIN_CLS_TYPE]) -> type[PLUGIN_CLS_TYPE]:
-            if not Plugin.__subclasscheck__(api_plugin):
-                raise NotValidPluginError("API插件主类必须继承Plugin类")
-            self.plugin_added_cache["plugin"] = api_plugin
-            self.pluginAPI_added_cache.append(apiName)
-            self.test_plugin(api_plugin) # type: ignore
-            return api_plugin
-
-        return _add_plugin_2_api
-
-    def add_packet_listener(self, pktID: int | list[int]) -> Callable[[Callable], Callable]:
-        """添加数据包监听器
-
+        添加数据包监听器
         将下面的方法作为一个MC数据包接收器
+        Tips: 只能在插件主类里的函数使用此装饰器!
 
         Args:
             pktID (int | list[int]): 数据包ID或多个ID
 
         Returns:
             Callable[[Callable], Callable]: 添加数据包监听器
         """
-        def deco(func):
+        def deco(func: Callable[[_SUPER_CLS, dict], bool]):
             if isinstance(pktID, int):
                 self.plugin_added_cache["packets"].append((pktID, func))
             else:
                 for i in pktID:
                     self.plugin_added_cache["packets"].append((i, func))
             return func
 
         return deco
 
-    def add_broadcast_listener(self, evt_name: str) -> Callable[[Callable], Callable[[Any], bool]]:
-        """添加广播事件监听器
+    def add_broadcast_listener(self, evt_name: str):
+        """
+        添加广播事件监听器
         将下面的方法作为一个广播事件接收器
+        Tips: 只能在插件主类里的函数使用此装饰器!
 
         Args:
             evt_name (str): 事件名
 
         Returns:
             Callable[[Callable], Callable]: 添加广播事件监听器
 
         原理:
         方法1 广播: hi, what's ur name? 附加参数=english_only
             - 方法2 接收到广播并被执行: 方法2(english_only) -> my name is Super. -> 收集表
 
         事件1 获取到 收集表 作为返回: ["my name is Super."]
         """
 
-        def deco(func: Callable[[Any], bool]) -> Callable[[Any], bool]:
+        def deco(func: Callable[[_SUPER_CLS, _TV], bool]) -> Callable[[_SUPER_CLS, _TV], bool]:
             if self.broadcast_evts_cache.get(evt_name):
                 self.broadcast_evts_cache[evt_name].append(func)
             else:
                 self.broadcast_evts_cache[evt_name] = [func]
             return func
 
         return deco
@@ -165,29 +135,14 @@
         if res:
             for f in res:
                 res2 = f(data)
                 if res2:
                     callback_list.append(res2)
         return callback_list
 
-    def test_plugin(self, plugin: type[Plugin]) -> None:
-        """测试插件是否符合要求
-
-        Args:
-            plugin (Plugin): 插件主类
-        """
-        if self.linked_frame is None:
-            # 很可能是直接单独运行此插件的代码.
-            Print.clean_print(f"插件主类信息({plugin.name}): ")
-            Print.clean_print(
-                f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
-            Print.clean_print(
-                f" - 数据包监听: {', '.join(str(i) for i in self._listen_packet_ids)}"
-            )
-
     @staticmethod
     def help(plugin: Plugin) -> None:
         """
         查看插件帮助.
         常用于查看 get_plugin_api() 方法获取到的插件实例的帮助.
         """
         plugin_docs = "<plugins.help>: " + plugin.name + "开放的API接口说明:\n"
```

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/__init__.py` & `tooldelta-0.6.2/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.6.2/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 "ToolDelta类式插件"
 import importlib
 import os
 import sys
 import traceback
 import zipfile
-from typing import TYPE_CHECKING, Callable, Union
+from typing import TYPE_CHECKING, Union, Any, TypeVar
 from ...color_print import Print
 from ...utils import Utils
 from ...cfg import Cfg
 from ...plugin_load import plugin_is_enabled, NotValidPluginError
 from ...constants import TOOLDELTA_CLASSIC_PLUGIN
 
 if TYPE_CHECKING:
     # 类型注释
     from ...frame import Frame
     from ...plugin_load.PluginGroup import PluginGroup
 
+__caches__ = {
+    "plugin": None,
+    "api_name": ""
+}
+
 class Plugin:
     "插件信息主类"
     name: str = ""
     version = (0, 0, 1)
     author = "?"
     description = "..."
 
@@ -30,14 +35,63 @@
     @property
     def data_path(self) -> str:
         "该插件的数据文件夹路径 (调用时直接创建数据文件夹)"
         path = os.path.join("插件数据文件", self.name)
         os.makedirs(path, exist_ok=True)
         return path
 
+_PLUGIN_CLS_TYPE = TypeVar("_PLUGIN_CLS_TYPE")
+
+def add_plugin(plugin: type[_PLUGIN_CLS_TYPE]) -> type[_PLUGIN_CLS_TYPE]:
+    """添加ToolDelta类式插件的插件主类
+
+    Args:
+        plugin (type[Plugin]): 插件主类
+
+    Raises:
+        NotValidPluginError: 插件主类必须继承Plugin类
+
+    Returns:
+        type[Plugin]: 插件主类
+    """
+    try:
+        if not Plugin.__subclasscheck__(plugin):
+            raise NotValidPluginError(f"插件主类必须继承Plugin类 而不是 {plugin}")
+    except TypeError as exc:
+        raise NotValidPluginError(
+            f"插件主类必须继承Plugin类 而不是 {plugin.__class__}") from exc
+    if __caches__["plugin"] is not None:
+        raise NotValidPluginError(
+            "调用了多次 @add_plugin"
+        )
+    __caches__["plugin"] = plugin
+    return plugin
+
+def add_plugin_as_api(apiName: str):
+    """添加ToolDelta类式插件主类, 同时作为API插件提供接口供其他插件进行使用
+
+    Args:
+        apiName (str): API名
+    """
+    def _add_plugin_2_api(api_plugin: type[_PLUGIN_CLS_TYPE]) -> type[_PLUGIN_CLS_TYPE]:
+        if not Plugin.__subclasscheck__(api_plugin):
+            raise NotValidPluginError("API插件主类必须继承Plugin类")
+        if __caches__["plugin"] is not None:
+            raise NotValidPluginError(
+                "调用了多次 @add_plugin"
+            )
+        __caches__["plugin"] = api_plugin
+        __caches__["api_name"] = apiName
+        return api_plugin
+
+    return _add_plugin_2_api
+
+
+# Plugin get and execute
+
 def read_plugins(plugin_grp: "PluginGroup") -> None:
     """读取插件
 
     Args:
         plugin_grp (PluginGroup): 插件组
     """
     PLUGIN_PATH = os.path.join("插件文件", TOOLDELTA_CLASSIC_PLUGIN)
@@ -81,107 +135,97 @@
         SystemExit: 插件名字不合法
         SystemExit: 插件配置文件报错
         SystemExit: 插件读取数据失败
 
     Returns:
         Union[None, Plugin]: 插件实例
     """
-    plugin_grp = plugin_group
-    if isinstance(plugin_grp, type(None)):
+    if isinstance(plugin_group, type(None)):
         raise ValueError("插件组未初始化读取")
-    if isinstance(plugin_grp.linked_frame, type(None)):
+    if isinstance(plugin_group.linked_frame, type(None)):
         raise ValueError("插件组未绑定框架")
+    plugin_group.plugin_added_cache["packets"].clear()
+    plugin_group.broadcast_evts_cache.clear()
+    __caches__["plugin"] = None
+    __caches__["api_name"] = ""
     try:
         if os.path.isfile(
             os.path.join(
                 "插件文件", TOOLDELTA_CLASSIC_PLUGIN, plugin_dirname, "__init__.py"
             )
         ):
-            importlib.__import__(plugin_dirname)
+            importlib.import_module(plugin_dirname)
         else:
             Print.print_war(f"{plugin_dirname} 文件夹 未发现插件文件, 跳过加载")
             return
-        Utils.simpleAssert(
-            plugin_grp.plugin_added_cache["plugin"] is not None,
-            NotValidPluginError(
+        none = None # ...
+        if __caches__["plugin"] == none:
+            raise NotValidPluginError(
                 "需要调用1次 @plugins.add_plugin 以注册插件主类, 然而没有调用"
-            ),
-        )
-        plugin: type[Plugin] = plugin_grp.plugin_added_cache["plugin"]
+            )
+        plugin: type[Plugin] = __caches__["plugin"] # type: ignore
         if plugin.name is None:
             raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
-        plugin_ins = plugin(plugin_grp.linked_frame)
+        plugin_ins = plugin(plugin_group.linked_frame)
         if isinstance(plugin_ins, type(None)) or plugin_ins.name == "":
             raise ValueError(f"插件主类 {plugin.__name__} 需要作者名")
-        plugin_grp.plugins.append([plugin_ins.name, plugin_ins])
+        plugin_group.plugins.append(plugin_ins)
         _v0, _v1, _v2 = plugin_ins.version
         for evt_name in (
             "on_def",
             "on_inject",
             "on_player_prejoin",
             "on_player_join",
             "on_player_message",
             "on_player_death",
             "on_player_leave",
             "on_frame_exit"
         ):
             if hasattr(plugin_ins, evt_name):
-                plugin_grp.plugins_funcs[evt_name].append(
+                plugin_group.plugins_funcs[evt_name].append(
                     [plugin_ins.name, getattr(plugin_ins, evt_name)]
                 )
         Print.print_suc(
             f"成功载入插件 {plugin_ins.name} 版本: {_v0}.{_v1}.{_v2} 作者：{plugin_ins.author}"
         )
-        plugin_grp.normal_plugin_loaded_num += 1
-        if plugin_grp.plugin_added_cache["packets"] != []:
-            for pktType, func in plugin_grp.plugin_added_cache["packets"]:
-                pfunc = getattr(plugin_ins, func.__name__)
-                if pfunc is None:
+        plugin_group.normal_plugin_loaded_num += 1
+        if plugin_group.plugin_added_cache["packets"] != []:
+            for pktType, func in plugin_group.plugin_added_cache["packets"]:
+                ins_func = getattr(plugin_ins, func.__name__)
+                if ins_func is None:
                     raise NotValidPluginError("数据包监听不能在主插件类以外定义")
-                plugin_grp._add_listen_packet_id(pktType)
-                plugin_grp._add_listen_packet_func(
-                    pktType, pfunc
+                plugin_group._add_listen_packet_id(pktType)
+                plugin_group._add_listen_packet_func(
+                    pktType, ins_func
                 )
-        if plugin_grp.pluginAPI_added_cache is not None:
-            for _api in plugin_grp.pluginAPI_added_cache:
-                if isinstance(_api, str):
-                    plugin_grp.plugins_api[_api] = plugin_ins
-                else:
-                    (apiName, api) = _api
-                    plugin_grp.plugins_api[apiName] = api(
-                        plugin_grp.linked_frame)
-        if plugin_grp.broadcast_evts_cache != {}:
-            for evt, funcs in plugin_grp.broadcast_evts_cache.items():
+        if __caches__["api_name"] != "":
+            plugin_group.plugins_api[__caches__["api_name"]] = plugin_ins
+        if plugin_group.broadcast_evts_cache != {}:
+            for evt, funcs in plugin_group.broadcast_evts_cache.items():
                 for func in funcs:
-                    bfunc = getattr(plugin_ins, func.__name__)
-                    if bfunc is not None:
-                        # 在插件主类以内定义了广播接收器
-                        func = bfunc
-                    plugin_grp._add_broadcast_evt(evt, func)
+                    ins_func = getattr(plugin_ins, func.__name__)
+                    if ins_func is None:
+                        raise NotValidPluginError("广播事件监听不能在主插件类以外定义")
+                    plugin_group._add_broadcast_evt(evt, ins_func)
         return plugin_ins
     except NotValidPluginError as err:
         Print.print_err(f"插件 {plugin_dirname} 不合法: {err.args[0]}")
         raise SystemExit from err
     except Cfg.ConfigError as err:
         Print.print_err(f"插件 {plugin_dirname} 配置文件报错：{err}")
         Print.print_err("你也可以直接删除配置文件, 重新启动ToolDelta以自动生成配置文件")
         raise SystemExit from err
     except Utils.SimpleJsonDataReader.DataReadError as err:
         Print.print_err(f"插件 {plugin_dirname} 读取数据失败: {err}")
-    except plugin_grp.linked_frame.SystemVersionException as err:
+    except plugin_group.linked_frame.SystemVersionException as err:
         Print.print_err(f"插件 {plugin_dirname} 需要更高版本的ToolDelta加载: {err}")
     except Exception as err:
         Print.print_err(f"加载插件 {plugin_dirname} 出现问题, 报错如下: ")
         Print.print_err("§c" + traceback.format_exc())
         raise SystemExit from err
-    finally:
-        plugin_grp.plugin_added_cache["plugin"] = None
-        plugin_grp.plugin_added_cache["packets"].clear()
-        plugin_grp.pluginAPI_added_cache.clear()
-        plugin_grp.broadcast_evts_cache.clear()
     return None
 
 def _unzip_plugin(zip_dir: str, exp_dir: str) -> None:
     """解压插件ZIP包
 
     Args:
         zip_dir (str): 压缩文件路径
```

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.6.2/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_load/utils.py` & `tooldelta-0.6.2/tooldelta/plugin_load/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_manager.py` & `tooldelta-0.6.2/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/plugin_market.py` & `tooldelta-0.6.2/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/starter.py` & `tooldelta-0.6.2/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/sys_args.py` & `tooldelta-0.6.2/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/urlmethod.py` & `tooldelta-0.6.2/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/tooldelta/utils.py` & `tooldelta-0.6.2/tooldelta/utils.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.6.1/PKG-INFO` & `tooldelta-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.6.1
+Version: 0.6.2
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,16 @@
 Requires-Dist: fcwslib (>=3.0.0,<4.0.0)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: mido (>=1.3.2,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (==5.9.8)
 Requires-Dist: pyspeedtest (==1.2.7)
 Requires-Dist: python-socketio (==5.11.1)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: pyyaml (==6.0.1)
+Requires-Dist: requests (==2.32.0)
 Requires-Dist: shellescape (>=3.8.1,<4.0.0)
 Requires-Dist: ujson (==5.9.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Project-URL: Repository, https://github.com/SuperScript-PRC/ToolDelta
 Description-Content-Type: text/markdown
 
 <h1 align="center">ToolDelta - Multi Platform Edition</h1>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.1 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.6.2 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: fcwslib (>=3.0.0,<4.0.0) Requires-Dist: flask
 (>=3.0.2,<4.0.0) Requires-Dist: mido (>=1.3.2,<2.0.0) Requires-Dist: pillow
 (>=10.2.0,<11.0.0) Requires-Dist: psutil (==5.9.8) Requires-Dist: pyspeedtest
-(==1.2.7) Requires-Dist: python-socketio (==5.11.1) Requires-Dist: requests
-(==2.31.0) Requires-Dist: shellescape (>=3.8.1,<4.0.0) Requires-Dist: ujson
-(==5.9.0) Requires-Dist: websocket-client (>=1.7.0,<2.0.0) Project-URL:
-Repository, https://github.com/SuperScript-PRC/ToolDelta Description-Content-
-Type: text/markdown
+(==1.2.7) Requires-Dist: python-socketio (==5.11.1) Requires-Dist: pyyaml
+(==6.0.1) Requires-Dist: requests (==2.32.0) Requires-Dist: shellescape
+(>=3.8.1,<4.0.0) Requires-Dist: ujson (==5.9.0) Requires-Dist: websocket-client
+(>=1.7.0,<2.0.0) Project-URL: Repository, https://github.com/SuperScript-PRC/
+ToolDelta Description-Content-Type: text/markdown
                ************ TToooollDDeellttaa -- MMuullttii PPllaattffoorrmm EEddiittiioonn ************
                                _[_R_e_l_e_a_s_e_s_][Stars]
                        _[_o_p_i_s_s_u_e_s_]_[_c_l_i_s_s_u_e_s_]_[_o_p_p_r_]_[_c_l_p_r_]
                TToooollDDeellttaa æ¯ä¾èµäº PPhhooeenniixxBBuuiillddeerr || NNeeoo OOmmeeggaa
     çå¤åè½æ©å±ç»ä»¶ï¼å¯ä»¥å è½½åç§åæ ·æè¶£çæä»¶ã
   TToooollDDeellttaa å¯ä»¥ä½¿å¾ä½ ç ?ä?¸?­?å??½?ç???ã???æ???ç???ä?¸??ç???ã???å??º?å?²?©?ç???ç?§??è?µ??æ??
                      çç©æ³ååè½æ´å å¤æ ·åã
```

