# Comparing `tmp/GameWorldNavigator-0.0.7.tar.gz` & `tmp/GameWorldNavigator-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWorldNavigator-0.0.7.tar", last modified: Mon May 27 06:03:14 2024, max compression
+gzip compressed data, was "GameWorldNavigator-0.0.7.1.tar", last modified: Thu May 30 14:27:42 2024, max compression
```

## Comparing `GameWorldNavigator-0.0.7.tar` & `GameWorldNavigator-0.0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.011303 GameWorldNavigator-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-05-27 06:03:13.979457 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/
--rw-rw-rw-   0        0        0      788 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      788 2024-05-27 06:03:14.010188 GameWorldNavigator-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.003390 GameWorldNavigator-0.0.7/gamenavigator/
--rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7/gamenavigator/__init__.py
--rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7/gamenavigator/config.py
--rw-rw-rw-   0        0        0     3376 2024-05-26 15:31:33.000000 GameWorldNavigator-0.0.7/gamenavigator/controller.py
-drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.009181 GameWorldNavigator-0.0.7/gamenavigator/core/
--rw-rw-rw-   0        0        0      136 2024-05-26 04:08:20.000000 GameWorldNavigator-0.0.7/gamenavigator/core/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7/gamenavigator/core/image.py
--rw-rw-rw-   0        0        0     3396 2024-05-26 04:26:37.000000 GameWorldNavigator-0.0.7/gamenavigator/core/interface.py
--rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7/gamenavigator/core/pos.py
--rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7/gamenavigator/core/rect.py
--rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7/gamenavigator/exception.py
--rw-rw-rw-   0        0        0    17020 2024-05-27 04:37:24.000000 GameWorldNavigator-0.0.7/gamenavigator/game_controller.py
--rw-rw-rw-   0        0        0     3183 2024-05-26 09:31:01.000000 GameWorldNavigator-0.0.7/gamenavigator/game_interface_controller.py
--rw-rw-rw-   0        0        0     4148 2024-05-26 11:24:27.000000 GameWorldNavigator-0.0.7/gamenavigator/image_recognition.py
--rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7/gamenavigator/keyboard_mouse_simulation.py
--rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7/gamenavigator/listener.py
--rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7/gamenavigator/log.py
--rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7/gamenavigator/ocr_recognition.py
--rw-rw-rw-   0        0        0       42 2024-05-27 06:03:14.011303 GameWorldNavigator-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-05-27 06:02:08.000000 GameWorldNavigator-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.302103 GameWorldNavigator-0.0.7.1/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.288026 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/
+-rw-rw-rw-   0        0        0      790 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 14:27:42.000000 GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7.1/LICENSE
+-rw-rw-rw-   0        0        0      790 2024-05-30 14:27:42.301411 GameWorldNavigator-0.0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.295901 GameWorldNavigator-0.0.7.1/gamenavigator/
+-rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7.1/gamenavigator/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7.1/gamenavigator/config.py
+-rw-rw-rw-   0        0        0     4997 2024-05-30 14:20:09.000000 GameWorldNavigator-0.0.7.1/gamenavigator/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:27:42.300631 GameWorldNavigator-0.0.7.1/gamenavigator/core/
+-rw-rw-rw-   0        0        0      149 2024-05-30 14:04:45.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/image.py
+-rw-rw-rw-   0        0        0     3766 2024-05-30 14:08:11.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/interface.py
+-rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/pos.py
+-rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7.1/gamenavigator/core/rect.py
+-rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7.1/gamenavigator/exception.py
+-rw-rw-rw-   0        0        0    17077 2024-05-28 08:45:58.000000 GameWorldNavigator-0.0.7.1/gamenavigator/game_controller.py
+-rw-rw-rw-   0        0        0     3237 2024-05-27 07:11:03.000000 GameWorldNavigator-0.0.7.1/gamenavigator/game_interface_controller.py
+-rw-rw-rw-   0        0        0     4148 2024-05-26 11:24:27.000000 GameWorldNavigator-0.0.7.1/gamenavigator/image_recognition.py
+-rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7.1/gamenavigator/keyboard_mouse_simulation.py
+-rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7.1/gamenavigator/listener.py
+-rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7.1/gamenavigator/log.py
+-rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7.1/gamenavigator/ocr_recognition.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:27:42.302103 GameWorldNavigator-0.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-05-30 14:27:02.000000 GameWorldNavigator-0.0.7.1/setup.py
```

### Comparing `GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/PKG-INFO` & `GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/SOURCES.txt` & `GameWorldNavigator-0.0.7.1/GameWorldNavigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/LICENSE` & `GameWorldNavigator-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/PKG-INFO` & `GameWorldNavigator-0.0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/__init__.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/__init__.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/controller.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/game_interface_controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,92 @@
-from ast import Tuple
-from re import I
-from typing import Any, Type, Union
-from .core import Interface, InterfaceAction as Action, InterfaceStep, Pos, Image
-from .game_controller import GameController
-from .game_interface_controller import GameInterfaceController
-
-class Controller:
-    def __init__(self, game_class: Union[str, None], game_name: str, root_inf: Interface) -> None:
-        self.game_controller = GameController(game_class, game_name)
-        self.inf_controller = GameInterfaceController(root_inf)
-    
-    def to_interface(self, inf_name: str) -> None:
-        """切换界面
+from functools import lru_cache
+from typing import Union, Optional, List, Dict, Tuple
+from collections import defaultdict, deque
 
-        Args:
-            inf_name (str): 想要前往的界面
-        """
-        target_inf = self.inf_controller.get_interface(inf_name)
-        steps = self.inf_controller.to_interface(inf_name)
-        
-        for step in steps:
-            self.__run_inf_step(step)
-        
-        self.inf_controller.set_current(inf_name)
-    
-    def __run_inf_step(self, step: InterfaceStep) -> None:
-        """运行界面步骤
-        
-        Args:
-            step (InterfaceStep): 界面步骤
+from .core import Interface, InterfaceStep, Image
+from .image_recognition import match_template
+from .log import logger
+
+
+class GameInterfaceController(object):
+    def __init__(self, current_inf: Interface) -> None:
+        self.current: Optional[Interface] = current_inf
+        self.name_to_inf: Dict[str, Interface] = dict()
+    
+    def add_interface(self, interface: Interface) -> None:
+        """ 添加界面 """
+        self.name_to_inf[interface.name] = interface
+    
+    def add_interfaces(self, interfaces: List[Interface]) -> None:
+        """ 添加界面 """
+        for interface in interfaces:
+            self.add_interface(interface)
+    
+    # 通过缓存加快查找速度
+    @lru_cache(maxsize=128)
+    def find_steps(self, start: str, target: str) -> List[InterfaceStep]:
+        """查找从start到target的路径
         
-        """
-        for action, arg in step:
-            match action:
-                case Action.MOUSE_CLICK:
-                    if isinstance(arg, tuple):
-                        raise TypeError("Invalid mouse click argument")
-                    self.__mouse_click(arg)
-                case Action.MOUSE_MOVE:
-                    if isinstance(arg, tuple):
-                        raise TypeError("Invalid mouse click argument")
-                    self.__mouse_move(arg)
-                case Action.MOUSE_DRAG:
-                    if not isinstance(arg, Pos):
-                        raise TypeError("Invalid mouse drag argument")
-                    self.__mouse_drag(arg)
-                case Action.KEYBOARD:
-                    if not isinstance(arg, (str, tuple)):
-                        raise TypeError("Invalid keyboard argument")
-                    self.__keyboard(arg)
-    
-    def __mouse_click(self, arg: Union[str, Image, Pos]) -> None:
-        """鼠标点击
+        从start界面开始,向父界面以及子界面搜索,直到找到target界面或者搜索完所有界面
 
         Args:
-            arg (Union[str, Image, Pos]): 要点击的元素,可以是文字,图像,位置
+            start (str): 当前界面的名称
+            target (str): 目标界面的名称
 
-        Raises:
-            TypeError: Invalid mouse click argument
+        Returns:
+            List[InterfaceStep]: 从start到target的路径
         """
-        if isinstance(arg, str):
-            self.game_controller.click_text(arg, y=5)
-        elif isinstance(arg, Image):
-            self.game_controller.click_image(arg.cv2_image)
-        elif isinstance(arg, Pos):
-            self.game_controller.click_pos(arg)
-        else:
-            raise TypeError("Invalid mouse click argument")
+        result = []
+        directions = []
+        
+        def dfs(cur: Interface, pre=None):
+            if cur.name == target:
+                return True
+            
+            for nex in cur.parents:
+                if nex == pre:
+                    continue
+                directions.append((0, nex.name))
+                if dfs(nex, cur):
+                    return True
+                directions.pop()
+                
+            
+            for nex in cur.children:
+                if nex == pre:
+                    continue
+                directions.append((1, nex.name))
+                if dfs(nex, cur):
+                    return True
+                directions.pop()
+            return False
+        
+        dfs(self.name_to_inf[start])
+        cur_inf = self.name_to_inf[start]
+        for _, name in directions:
+            inf = cur_inf.get_interface(name)
+            if inf is None:
+                raise ValueError(f"<界面{cur_inf.name}>找不到界面<{name}>")
+            result.append(cur_inf.get_step(inf))
+            cur_inf = inf
+        return result
+    
+    def get_interface(self, inf_name: str) -> Interface:
+        return self.name_to_inf[inf_name]
+    
+    def to_interface(self, interface_name: str) -> List[InterfaceStep]:
+        current_inf = self.current
+        if current_inf is None:
+            logger.error("当前界面为None,请初始化当前界面")
+            return []
+        if interface_name == current_inf.name:
+            logger.debug(f"当前界面为{current_inf.name},无需切换")
+            return []
+        steps = self.find_steps(current_inf.name, interface_name)
+        return steps
+
+    def set_current(self, inf_name: str):
+        self.current = self.name_to_inf[inf_name]
     
-    def __mouse_move(self, arg: Union[str, Image, Pos]) -> None:
-        """移动鼠标
+    def exists(self, name: str) -> bool:
+        return name in self.name_to_inf
 
-        Args:
-            arg (Union[str, Image, Pos]): 鼠标可以移动到文字,图像,位置
-        """
-        if isinstance(arg, Image):
-            self.game_controller.mouse_move_to(arg.cv2_image, 0.0)
-        else:
-            self.game_controller.mouse_move_to(arg, 0.0)
-    
-    def __mouse_drag(self, arg):
-        pass
-    
-    def __keyboard(self, arg: str | tuple) -> None:
-        if isinstance(arg, str):
-            self.game_controller.down_keyboard_time(arg, 0.0)
-        elif isinstance(arg, tuple):
-            self.game_controller.down_keyboard_time(*arg)
```

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/core/image.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/core/image.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/core/pos.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/core/pos.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/core/rect.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/core/rect.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/game_controller.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/game_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 import ctypes
 import time
 from threading import Thread
+from concurrent.futures import ThreadPoolExecutor, Future
 from typing import Union, Optional
 
 import cv2
 import win32api
 import win32con
 import win32gui
 import win32print
 from PIL import ImageGrab
 from cv2.typing import MatLike
 from numpy import ndarray, array
 
 from . import log
 from .core import Pos, Rect
-from .exception import TemplateMathingFailure, WindowOutOfBoundsError, TextMatchingFailure
+from .exception import (
+    TemplateMathingFailure,
+    WindowOutOfBoundsError,
+    TextMatchingFailure,
+)
 from .image_recognition import match_template
-from .keyboard_mouse_simulation import (mouse_click_position, mouse_move_to, mouse_scroll,
-                                        keyboard_press, keyboard_down, keyboard_up, mouse_drag)
-from .ocr_recognition import (get_text_position, get_text_direction_position)
+from .keyboard_mouse_simulation import (
+    mouse_click_position,
+    mouse_move_to,
+    mouse_scroll,
+    keyboard_press,
+    keyboard_down,
+    keyboard_up,
+    mouse_drag,
+)
+from .ocr_recognition import get_text_position, get_text_direction_position
 
 
 def _get_screen_size():
-    """ 电脑缩放后的分辨率 """
+    """电脑缩放后的分辨率"""
     w = win32api.GetSystemMetrics(0)
     h = win32api.GetSystemMetrics(1)
     return w, h
 
 
 def _get_read_size():
-    """ 获取电脑真实分辨率 """
+    """获取电脑真实分辨率"""
     hdc = win32gui.GetDC(0)
     w = win32print.GetDeviceCaps(hdc, win32con.DESKTOPHORZRES)
     h = win32print.GetDeviceCaps(hdc, win32con.DESKTOPVERTRES)
     return w, h
 
 
 def _get_scaling() -> float:
-    """ 获取电脑缩放率 """
+    """获取电脑缩放率"""
     return round(_get_read_size()[0] / _get_screen_size()[0], 2)
 
 
+THREAD_POOL = ThreadPoolExecutor(max_workers=100)
+
+
 class Game:
     def __init__(self, game_class: Union[str, None], game_name: str):
         """
         :param game_class: 游戏类名
         :param game_name: 游戏名称
         """
         self.screenshot: Optional[ndarray] = None
@@ -83,55 +98,54 @@
         return ctypes.windll.user32.GetDpiForWindow(self._hwnd) / 96.0
 
     @property
     def name(self) -> str:
         return self._game_name
 
     def set_foreground(self) -> None:
-        """ 设置游戏到前台API """
+        """设置游戏到前台API"""
         win32gui.ShowWindow(self._hwnd, win32con.SW_RESTORE)
         win32gui.SetForegroundWindow(self._hwnd)
 
     def get_screenshot(self) -> ndarray:
-        """ 游戏截图API """
+        """游戏截图API"""
         grab = ImageGrab.grab(bbox=(self.get_rect().rect()))
         img = array(grab)
         img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
         self.screenshot = img
         return img
 
     def get_rect(self) -> Rect:
-        """ 获取游戏的矩形 """
+        """获取游戏的矩形"""
         x1, y1, x2, y2 = win32gui.GetWindowRect(self._hwnd)
         s = _get_scaling()  # 电脑缩放率
         x1, y1 = int(x1 * s), int(y1 * s)
         x2, y2 = int(x2 * s), int(y2 * s)
         return Rect(x1, y1, x2, y2)
-    
+
     def get_image_pos(self, image: Union[str, ndarray]) -> Pos:
         """获取游戏内图片位置API
 
         Args:
             image (Union[str, ndarray]): 模板图
         """
         _, _, _, max_loc = match_template(self.get_screenshot(), image)
         pos = Pos(max_loc[0], max_loc[1])
         return pos
-    
+
     def get_text_pos(self, text: str, direction: str = "center") -> Pos:
         """获取游戏内文字位置API
 
         Args:
             text (str): 文字
             direction (str, optional): 文字的位置方向 [left, center, right]. Defaults to "center".
         """
         positions = get_text_position(self.get_screenshot(), text)
         pos = get_text_direction_position(positions, direction)
         return pos
-        
 
 
 class GameController:
     def __init__(self, game_class: Union[str, None], game_name: str):
         """
         将debug设置为True后需要设置filename才会将调试信息保存
 
@@ -189,58 +203,60 @@
         if not isinstance(position, str):
             raise TypeError("position must is str type")
         try:
             self._click_text(text, position, **kwargs)
         except TextMatchingFailure:
             raise
 
-    def down_keyboard_time(self, key: str, stop_time: float, thread=False) -> Union[None, Thread]:
-        """模拟按压键盘的时间
-
-        开启线程后将在子线程中运行从而不阻塞主线程，因为这个按压时间是通过time.sleep()实现的
+    def down_keyboard_time(
+        self, key: str, stop_time: float, thread=True
+    ) -> Union[None, Future]:
+        """模拟键盘按压
 
         Args:
-            key (str): 键盘按键
-            stop_time (float): 按压时间
-            thread (bool): 开启线程(default False)
+            key (str): 按键
+            stop_time (float): 按压时长
+            thread (bool, optional): 是否开启线程. Defaults to True.
+
+        Raises:
+            TypeError: 类型错误
 
         Returns:
-            None | Thread
+            Union[None, Future]: 若开启线程则会返回Future对象,否则返回None
         """
         if not isinstance(stop_time, float):
             raise TypeError("param stop_time must is float type")
         if not isinstance(thread, bool):
             raise TypeError("param thread must is bool type")
         self.set_foreground()
 
         def func():
             keyboard_down(key)
             time.sleep(stop_time)
             keyboard_up(key)
 
         if thread:
-            t = Thread(target=func)
-            t.start()
-            return t
+            res = THREAD_POOL.submit(func)
+            return res
             # 运行子线程并且返回子线程
         func()
         # 阻塞当前线程直到达到按压时长
         return None
 
     def get_screenshot(self) -> ndarray:
-        """ 获取游戏截图 """
+        """获取游戏截图"""
         return self.game.get_screenshot()
 
     def press(self, key: str) -> None:
-        """ 模拟键盘按键按压API """
+        """模拟键盘按键按压API"""
         self.set_foreground()
         keyboard_press(key)
 
     def set_foreground(self) -> None:
-        """ 设置游戏到前台 """
+        """设置游戏到前台"""
         hwnd = win32gui.GetForegroundWindow()
         text = win32gui.GetWindowText(hwnd)
         if text != self.game.name:
             self.game.set_foreground()
             time.sleep(1)
 
     @property
@@ -303,20 +319,20 @@
         self.set_foreground()
         try:
             self._wait_image(*images, **kwargs)
         except TimeoutError:
             raise
 
     def _click_pos(self, pos: Pos) -> None:
-        """ 点击游戏内某个坐标 """
+        """点击游戏内某个坐标"""
         game_pos = self._to_global_pos(pos)
         mouse_click_position(game_pos)
 
     def _click_image(self, *images: Union[str, ndarray, MatLike], **kwargs) -> None:
-        """ 点击游戏内图片 """
+        """点击游戏内图片"""
         x = kwargs.get("x", 0)
         y = kwargs.get("y", 0)
         threshold = kwargs.get("threshold", 0.8)
         mode = kwargs.get("mode", "color")
         if not isinstance(x, int):
             raise TypeError("param x must is int type")
         if not isinstance(y, int):
@@ -347,15 +363,15 @@
                 center += Pos(x, y)
                 self.click_pos(center)
                 return
         log.error(f"template matching failure, max value is {v}")
         raise TemplateMathingFailure(f"Threshold: {v} < {threshold}, GamePos: {p}")
 
     def _click_text(self, text: str, position: str = "center", **kwargs) -> None:
-        """ 点击游戏内文字 """
+        """点击游戏内文字"""
         x = kwargs.get("x", 0)
         y = kwargs.get("y", 0)
         add_pos = Pos(x, y)
         positions = get_text_position(self.game.get_screenshot(), text)
         if positions.size == 0:
             raise TextMatchingFailure(f"The text does not exist in the game")
             # 没有匹配到相关的文字
@@ -407,25 +423,27 @@
             return pos
         rect = self.game.get_rect()
         x1, y1 = pos.x, pos.y
         x2, y2 = x1 + rect.left, y1 + rect.top
         # 坐标转换成游戏内坐标
         if x2 < rect.left or x2 > rect.right or y2 < rect.top or y2 > rect.bottom:
             log.error(f"The given coordinate ({x2}, {y2}) is outside")
-            raise WindowOutOfBoundsError(f"The given coordinate ({x2}, {y2}) is outside "
-                                         f"the game window bounds "
-                                         f"({rect.left}, {rect.top}) - ({rect.right}, {rect.bottom})")
+            raise WindowOutOfBoundsError(
+                f"The given coordinate ({x2}, {y2}) is outside "
+                f"the game window bounds "
+                f"({rect.left}, {rect.top}) - ({rect.right}, {rect.bottom})"
+            )
             # 给出的坐标超出游戏窗口范围
         global_pos = Pos(x2, y2)
         return global_pos
 
     def _wait_image(self, *images: Union[str, ndarray], **kwargs) -> None:
         """等待图片
         阻塞线程等待图片出现或者超市
-        
+
         Args:
             *images (Union[str, ndarray]): 图片路径,图片,图片模板
             all (bool, optional): 是否需要所有图片同时出现. Defaults to False.
             threshold (float, optional): 匹配阈值. Defaults to 0.8.
             mode (str, optional): 匹配模式. Defaults to "color".
             timeout (int, optional): 超时时间. Defaults to 60.
             spacing (int, optional): 图片间隔时间. Defaults to 1.
```

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/image_recognition.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/image_recognition.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/keyboard_mouse_simulation.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/keyboard_mouse_simulation.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/listener.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/listener.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/log.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/log.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/gamenavigator/ocr_recognition.py` & `GameWorldNavigator-0.0.7.1/gamenavigator/ocr_recognition.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.7/setup.py` & `GameWorldNavigator-0.0.7.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="GameWorldNavigator",
-    version="0.0.7",
+    version="0.0.7.1",
     author="NanJunLYS",
     author_email="18906571516@163.com",
     description="A framework for game automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JunNanLYS/GameWorldNavigator",
     packages=setuptools.find_packages(),
```

