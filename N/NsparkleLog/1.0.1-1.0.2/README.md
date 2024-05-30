# Comparing `tmp/NsparkleLog-1.0.1.tar.gz` & `tmp/NsparkleLog-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NsparkleLog-1.0.1.tar", last modified: Sun May 26 15:10:32 2024, max compression
+gzip compressed data, was "NsparkleLog-1.0.2.tar", last modified: Thu May 30 13:49:58 2024, max compression
```

## Comparing `NsparkleLog-1.0.1.tar` & `NsparkleLog-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.811286 NsparkleLog-1.0.1/
--rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.636088 NsparkleLog-1.0.1/NsparkleLog/
--rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.1/NsparkleLog/Interfaces.py
--rw-rw-rw-   0        0        0      265 2024-05-26 15:10:04.000000 NsparkleLog-1.0.1/NsparkleLog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.803307 NsparkleLog-1.0.1/NsparkleLog/core/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.1/NsparkleLog/core/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.1/NsparkleLog/core/_excformat.py
--rw-rw-rw-   0        0        0     1509 2024-05-26 14:57:02.000000 NsparkleLog-1.0.1/NsparkleLog/core/_formatter.py
--rw-rw-rw-   0        0        0     4096 2024-05-26 15:08:14.000000 NsparkleLog-1.0.1/NsparkleLog/core/_handler.py
--rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.1/NsparkleLog/core/_level.py
--rw-rw-rw-   0        0        0     5985 2024-05-26 13:00:56.000000 NsparkleLog-1.0.1/NsparkleLog/core/_logger.py
--rw-rw-rw-   0        0        0     1380 2024-05-26 15:07:19.000000 NsparkleLog-1.0.1/NsparkleLog/core/_manager.py
--rw-rw-rw-   0        0        0      312 2024-05-26 14:43:06.000000 NsparkleLog-1.0.1/NsparkleLog/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.805303 NsparkleLog-1.0.1/NsparkleLog/plugins/
--rw-rw-rw-   0        0        0      450 2024-05-20 15:11:32.000000 NsparkleLog-1.0.1/NsparkleLog/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.1/NsparkleLog/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.808294 NsparkleLog-1.0.1/NsparkleLog/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.1/NsparkleLog/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.1/NsparkleLog/utils/_color.py
--rw-rw-rw-   0        0        0      178 2024-05-26 13:01:00.000000 NsparkleLog-1.0.1/NsparkleLog/utils/_types.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:10:32.809291 NsparkleLog-1.0.1/NsparkleLog.egg-info/
--rw-rw-rw-   0        0        0     3538 2024-05-26 15:10:31.000000 NsparkleLog-1.0.1/NsparkleLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2024-05-26 15:10:31.000000 NsparkleLog-1.0.1/NsparkleLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:10:31.000000 NsparkleLog-1.0.1/NsparkleLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 15:10:31.000000 NsparkleLog-1.0.1/NsparkleLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3538 2024-05-26 15:10:32.809291 NsparkleLog-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 15:10:32.811286 NsparkleLog-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.798913 NsparkleLog-1.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-25 15:37:29.000000 NsparkleLog-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.553981 NsparkleLog-1.0.2/NsparkleLog/
+-rw-rw-rw-   0        0        0      148 2024-05-26 13:00:49.000000 NsparkleLog-1.0.2/NsparkleLog/Interfaces.py
+-rw-rw-rw-   0        0        0      265 2024-05-30 13:32:00.000000 NsparkleLog-1.0.2/NsparkleLog/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-05-30 13:22:36.000000 NsparkleLog-1.0.2/NsparkleLog/_env.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.768975 NsparkleLog-1.0.2/NsparkleLog/core/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 NsparkleLog-1.0.2/NsparkleLog/core/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 NsparkleLog-1.0.2/NsparkleLog/core/_excformat.py
+-rw-rw-rw-   0        0        0     1467 2024-05-30 12:50:00.000000 NsparkleLog-1.0.2/NsparkleLog/core/_formatter.py
+-rw-rw-rw-   0        0        0     4026 2024-05-30 13:37:07.000000 NsparkleLog-1.0.2/NsparkleLog/core/_handler.py
+-rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 NsparkleLog-1.0.2/NsparkleLog/core/_level.py
+-rw-rw-rw-   0        0        0     5799 2024-05-30 13:32:46.000000 NsparkleLog-1.0.2/NsparkleLog/core/_logger.py
+-rw-rw-rw-   0        0        0     1337 2024-05-30 12:50:46.000000 NsparkleLog-1.0.2/NsparkleLog/core/_manager.py
+-rw-rw-rw-   0        0        0      312 2024-05-26 14:43:06.000000 NsparkleLog-1.0.2/NsparkleLog/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.770969 NsparkleLog-1.0.2/NsparkleLog/plugins/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.2/NsparkleLog/plugins/__init__.py
+-rw-rw-rw-   0        0        0      824 2024-05-30 13:02:42.000000 NsparkleLog-1.0.2/NsparkleLog/plugins/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.774958 NsparkleLog-1.0.2/NsparkleLog/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 NsparkleLog-1.0.2/NsparkleLog/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 NsparkleLog-1.0.2/NsparkleLog/utils/_color.py
+-rw-rw-rw-   0        0        0      178 2024-05-26 13:01:00.000000 NsparkleLog-1.0.2/NsparkleLog/utils/_types.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:49:58.775957 NsparkleLog-1.0.2/NsparkleLog.egg-info/
+-rw-rw-rw-   0        0        0     3676 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2024-05-30 13:49:56.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 13:49:55.000000 NsparkleLog-1.0.2/NsparkleLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3676 2024-05-30 13:49:58.776954 NsparkleLog-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:49:58.798913 NsparkleLog-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      650 2024-05-26 13:01:15.000000 NsparkleLog-1.0.2/setup.py
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog/core/_excformat.py` & `NsparkleLog-1.0.2/NsparkleLog/core/_excformat.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.1/NsparkleLog/core/_formatter.py` & `NsparkleLog-1.0.2/NsparkleLog/core/_formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from NsparkleLog.utils._types import AnyStr, Level
 from NsparkleLog.dependencies import datetime as dt , time
 from NsparkleLog.core._level import _levelToName
 from NsparkleLog.utils._color import Color
+from NsparkleLog._env import default_format
 
 class Formatter:
-    def __init__(self,colorMode:bool = False, fmt: str = "{localtime}.{msec} | {level:<7} | {threadName} | {name}.{funcName} | {filename}:{lineno} - {message}") -> None:
+    def __init__(self,colorMode:bool = False, fmt: str = default_format) -> None:
         self._fmt = fmt
         self.colorMode = colorMode
 
     def format(self, 
         name: str,
         threadName: str,
         filename: str,
         lineno: int,
         funcName: str,
         moduleName: str,
         message: AnyStr, 
         level: Level, 
         color: str,
         ) -> str:
-        msec = dt.now().microsecond // 1000
+        msec = dt.now().microsecond // 1000 
         utcmsec = time.time() * 1000
         timestamp = f"{dt.now().strftime('%Y-%m-%d %H:%M:%S')}"
         utctime = time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime())
         formatted_msg = self._fmt.format(
             timestamp=timestamp,
             msec=msec,
             utcmsec=utcmsec,
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog/core/_handler.py` & `NsparkleLog-1.0.2/NsparkleLog/core/_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from NsparkleLog.dependencies import stdout, stderr , threading , queue ,os , atexit
+from NsparkleLog.dependencies import stdout, stderr , threading , queue ,os
 from NsparkleLog.utils._types import Stream, AnyStr, Level
 from NsparkleLog.core._level import Levels, _levelToName
 from NsparkleLog.core._formatter import Formatter
 
+def isMainThreadAlive():
+    return threading.main_thread().is_alive()
 
 class Writer:
     """
     日志写入器
     """
     lock = threading.Lock()
 
@@ -83,43 +85,39 @@
     def __init__(self, filename: str, mode: str = "a+", encoding: str = "utf-8") -> None:
         super().__init__()
         self.filename = filename
         self.mode = mode
         self.encoding = encoding
         self.lock = threading.Lock()
         self.queue = queue.Queue()
-        self.stop_event = threading.Event()
         self.writeThread = threading.Thread(target=self.writeToFile)
         self.writeThread.start()
 
     def handle(self, name: str, threadName: str, filename: str, lineno: int, funcName: str, moduleName: str, message: AnyStr, level: Level, color: str) -> None:
         string = super().handle(name, threadName, filename, lineno, funcName, moduleName, message, level, color)
         if level >= self.level:
            self.queue.put(string)
         return
 
     def writeToFile(self) -> None:
         with open(self.filename, self.mode, encoding=self.encoding) as f:
-            while not self.stop_event.is_set() or not self.queue.empty():
+            while isMainThreadAlive():
                 try:
                     string = self.queue.get(timeout=1)  # 使用timeout来避免忙等
                     with self.lock:
                         f.write(string + "\n")
                         f.flush()
                     self.queue.task_done()
                 except queue.Empty:
-                    pass
+                    if  not isMainThreadAlive():
+                        break
+                    else:
+                        continue
                 except Exception as e:
                     stderr.write(f"{e}\n")
-
-    def __del__(self) -> None:
-        self.close()
-
-    def close(self) -> None:
-        self.stop_event.set()
-        self.writeThread.join()  # 等待写入线程退出
+        
 
 class RotatingFileHandler:
     """
     日志文件按大小轮换写入器
     """
     pass
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog/core/_logger.py` & `NsparkleLog-1.0.2/NsparkleLog/core/_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from NsparkleLog.utils._types import Level , AnyStr
 from NsparkleLog.core._level import Levels, _nameToLevel , _levelToName
 from NsparkleLog.core._handler import Handler
 from NsparkleLog.dependencies import threading , stderr , inspect , os , traceback
 from NsparkleLog.utils._color import _Color
+from NsparkleLog.plugins.helpers import Deprecated
 
 class Logger:
     def __init__(self,
     name: str = "main",
     level = Levels.ON,
     colorLevel: dict[Level, str] = {
         Levels.TRACE: "bd_grey",
@@ -44,21 +45,14 @@
                 funcName = frame.f_code.co_name # type: ignore
                 for handler in self.handlers:
                     handler.handle(self.name, threadName, filename, lineno, funcName, moduleName, message, level, color, **kwargs)
         except Exception as e:
             err_msg = traceback.format_exc()
             stderr.write(f"{err_msg}\n")
 
-    def close(self) -> None:
-        """
-        如果只用StreamHandler,则不需要调用此方法,否则必须调用来确保线程被安全关闭
-        """
-        for handler in self.handlers:
-            handler.close()
-
     def setLevel(self,level:Level):
         """
         设置日志等级
         """
         if level in _levelToName:
             with self.lock:
                 if _levelToName[level] == "OFF":
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog/core/_manager.py` & `NsparkleLog-1.0.2/NsparkleLog/core/_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from NsparkleLog.core._logger import Logger
 from NsparkleLog.dependencies import threading
 from NsparkleLog.utils._types import Level
 from NsparkleLog.core._level import Levels
 from NsparkleLog.core._handler import StreamHandler , Formatter
+from NsparkleLog._env import default_format
 
 class LogManager:
     loggers:set[Logger] = set()
     lock = threading.Lock()
 
     @classmethod
     def GetLogger(cls, 
@@ -24,13 +25,13 @@
         ):
         with cls.lock:
             logger = next((logger for logger in cls.loggers if logger.name == name),None)
             if logger is None:
                 logger = Logger(name,level,colorLevel=colorLevel)
                 console = StreamHandler()
                 console.setLevel(level)
-                console.setFormatter(Formatter(colorMode=colorMode,fmt="{localtime}.{msec} | {level:<7} | {threadName} | {name}.{funcName} | {filename}:{lineno} - {message}"))
+                console.setFormatter(Formatter(colorMode=colorMode,fmt=default_format))
                 logger.addHandler(console)
                 cls.loggers.add(logger)
                 return logger
             else:
                 return logger
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog/utils/_color.py` & `NsparkleLog-1.0.2/NsparkleLog/utils/_color.py`

 * *Files identical despite different names*

### Comparing `NsparkleLog-1.0.1/NsparkleLog.egg-info/PKG-INFO` & `NsparkleLog-1.0.2/NsparkleLog.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.1
+Version: 1.0.2
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,17 +35,19 @@
 
 logger.trace("test")
 logger.debug("test")
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
-
 ```
 
+[2024/5/30 21:33]
+# 日志库不用再需要显示调用close方法来释放资源,主线程退出后会自动释放资源
+
 # 更新了setLevel接口用于设置日志级别过滤
 
 - 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
 
 ```python
 from NsparkleLog import logger
 from NsparkleLog.core._level import Levels
@@ -92,15 +94,15 @@
 logger.error("Error message")
 logger.fatal("fatal message")
 
 # 别忘了显示调用close方法释放资源
 filehandler.close()
 ```
 
-# close方法写在了logger中，可以直接调用logger.close()方法来释放资源
+# close方法写在了logger中，可以直接调用logger.close()方法来释放资源 [depercated]
 
 ```python
 from NsparkleLog import logger
 from NsparkleLog.core._handler import FileHandler
 from NsparkleLog.core._formatter import Formatter
 
 filehandler = FileHandler(filename="test.log", mode="a+")
```

### Comparing `NsparkleLog-1.0.1/NsparkleLog.egg-info/SOURCES.txt` & `NsparkleLog-1.0.2/NsparkleLog.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 setup.py
 NsparkleLog/Interfaces.py
 NsparkleLog/__init__.py
+NsparkleLog/_env.py
 NsparkleLog/dependencies.py
 NsparkleLog.egg-info/PKG-INFO
 NsparkleLog.egg-info/SOURCES.txt
 NsparkleLog.egg-info/dependency_links.txt
 NsparkleLog.egg-info/top_level.txt
 NsparkleLog/core/__init__.py
 NsparkleLog/core/_excformat.py
 NsparkleLog/core/_formatter.py
 NsparkleLog/core/_handler.py
 NsparkleLog/core/_level.py
 NsparkleLog/core/_logger.py
 NsparkleLog/core/_manager.py
-NsparkleLog/plugins/DecoratorsTools.py
 NsparkleLog/plugins/__init__.py
+NsparkleLog/plugins/helpers.py
 NsparkleLog/utils/__init__.py
 NsparkleLog/utils/_color.py
 NsparkleLog/utils/_types.py
```

### Comparing `NsparkleLog-1.0.1/PKG-INFO` & `NsparkleLog-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NsparkleLog
-Version: 1.0.1
+Version: 1.0.2
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,17 +35,19 @@
 
 logger.trace("test")
 logger.debug("test")
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
-
 ```
 
+[2024/5/30 21:33]
+# 日志库不用再需要显示调用close方法来释放资源,主线程退出后会自动释放资源
+
 # 更新了setLevel接口用于设置日志级别过滤
 
 - 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
 
 ```python
 from NsparkleLog import logger
 from NsparkleLog.core._level import Levels
@@ -92,15 +94,15 @@
 logger.error("Error message")
 logger.fatal("fatal message")
 
 # 别忘了显示调用close方法释放资源
 filehandler.close()
 ```
 
-# close方法写在了logger中，可以直接调用logger.close()方法来释放资源
+# close方法写在了logger中，可以直接调用logger.close()方法来释放资源 [depercated]
 
 ```python
 from NsparkleLog import logger
 from NsparkleLog.core._handler import FileHandler
 from NsparkleLog.core._formatter import Formatter
 
 filehandler = FileHandler(filename="test.log", mode="a+")
```

### Comparing `NsparkleLog-1.0.1/setup.py` & `NsparkleLog-1.0.2/setup.py`

 * *Files identical despite different names*

