# Comparing `tmp/pyprland-2.3.4.tar.gz` & `tmp/pyprland-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.3.4.tar", max compression
+gzip compressed data, was "pyprland-2.3.5.tar", max compression
```

## Comparing `pyprland-2.3.4.tar` & `pyprland-2.3.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.4/LICENSE
--rw-r--r--   0        0        0     5553 2024-05-23 18:58:37.218905 pyprland-2.3.4/README.md
--rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/__init__.py
--rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.4/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.4/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4848 2024-05-19 09:02:05.262228 pyprland-2.3.4/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.4/pyprland/adapters/units.py
--rw-r--r--   0        0        0    18490 2024-05-22 23:20:39.841357 pyprland-2.3.4/pyprland/command.py
--rw-r--r--   0        0        0     8849 2024-05-20 16:29:06.584044 pyprland-2.3.4/pyprland/common.py
--rw-r--r--   0        0        0     8097 2024-05-24 21:47:53.805458 pyprland-2.3.4/pyprland/ipc.py
--rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.4/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2723 2024-05-17 21:51:17.035559 pyprland-2.3.4/pyprland/plugins/gbar.py
--rw-r--r--   0        0        0     2657 2024-05-19 00:11:17.726169 pyprland-2.3.4/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.4/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.4/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     2743 2024-05-23 22:10:42.465750 pyprland-2.3.4/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0      853 2024-05-23 17:45:08.310387 pyprland-2.3.4/pyprland/plugins/magnify.py.rej
--rw-r--r--   0        0        0    12344 2024-05-23 17:45:08.310387 pyprland-2.3.4/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     4043 2024-05-23 22:04:00.478257 pyprland-2.3.4/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    32579 2024-05-24 22:33:09.046321 pyprland-2.3.4/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2937 2024-05-24 22:33:09.046321 pyprland-2.3.4/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     3409 2024-05-24 22:33:09.049654 pyprland-2.3.4/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.4/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     6118 2024-05-24 16:27:21.239418 pyprland-2.3.4/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.4/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.4/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.4/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.4/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.4/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5828 2024-05-20 14:35:57.473856 pyprland-2.3.4/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.4/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0     1471 2024-05-23 19:18:57.916054 pyprland-2.3.4/pyprland/types.py
--rw-r--r--   0        0        0       42 2024-05-24 22:55:26.130770 pyprland-2.3.4/pyprland/version.py
--rw-r--r--   0        0        0     2124 2024-05-24 22:55:26.127436 pyprland-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     6092 1970-01-01 00:00:00.000000 pyprland-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.3.5/LICENSE
+-rw-r--r--   0        0        0     5905 2024-05-28 12:43:42.360950 pyprland-2.3.5/README.md
+-rw-r--r--   0        0        0       24 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-16 19:14:17.148810 pyprland-2.3.5/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      386 2024-05-16 19:14:17.148810 pyprland-2.3.5/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4848 2024-05-19 09:02:05.262228 pyprland-2.3.5/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1462 2024-05-16 20:28:22.384986 pyprland-2.3.5/pyprland/adapters/units.py
+-rw-r--r--   0        0        0    18490 2024-05-22 23:20:39.841357 pyprland-2.3.5/pyprland/command.py
+-rw-r--r--   0        0        0     9143 2024-05-30 18:08:55.679971 pyprland-2.3.5/pyprland/common.py
+-rw-r--r--   0        0        0     8437 2024-05-28 14:09:11.312946 pyprland-2.3.5/pyprland/ipc.py
+-rw-r--r--   0        0        0       49 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      115 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1658 2024-05-16 20:12:25.826075 pyprland-2.3.5/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1370 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     3077 2024-05-30 17:37:08.270783 pyprland-2.3.5/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2657 2024-05-19 00:11:17.726169 pyprland-2.3.5/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     8084 2024-05-18 12:50:01.915976 pyprland-2.3.5/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1731 2024-05-16 20:31:35.359564 pyprland-2.3.5/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     2743 2024-05-23 22:10:42.465750 pyprland-2.3.5/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0    12344 2024-05-23 17:45:08.310387 pyprland-2.3.5/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3817 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     3970 2024-05-28 12:43:42.360950 pyprland-2.3.5/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    32875 2024-05-28 12:47:20.865391 pyprland-2.3.5/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2937 2024-05-24 22:33:09.046321 pyprland-2.3.5/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     3409 2024-05-24 22:33:09.049654 pyprland-2.3.5/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     4036 2024-05-18 13:07:36.207295 pyprland-2.3.5/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     6118 2024-05-24 16:27:21.239418 pyprland-2.3.5/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1103 2024-05-16 20:02:45.022300 pyprland-2.3.5/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4245 2024-05-18 12:58:41.979853 pyprland-2.3.5/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4804 2024-05-16 20:40:18.898697 pyprland-2.3.5/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      570 2024-05-16 19:14:17.152144 pyprland-2.3.5/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1120 2024-05-16 19:55:58.745845 pyprland-2.3.5/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5828 2024-05-20 14:35:57.473856 pyprland-2.3.5/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2496 2024-05-16 19:55:44.465502 pyprland-2.3.5/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0     1752 2024-05-28 14:06:42.326450 pyprland-2.3.5/pyprland/types.py
+-rw-r--r--   0        0        0     1192 2024-05-30 18:10:47.658835 pyprland-2.3.5/pyprland/utils.py
+-rw-r--r--   0        0        0       42 2024-05-30 18:12:17.840601 pyprland-2.3.5/pyprland/version.py
+-rw-r--r--   0        0        0     2124 2024-05-30 18:12:17.833934 pyprland-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 pyprland-2.3.5/PKG-INFO
```

### Comparing `pyprland-2.3.4/LICENSE` & `pyprland-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/README.md` & `pyprland-2.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,21 +64,30 @@
 <details>
 <summary>
 Latest major changes
 </summary>
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
+### 2.3
+
+- Supports _Hyprland > 0.40.0_
+- Improved code kwaleetee
+- [monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) allows general monitor settings
+- [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
+  - better multi-window support
+  - better `preserve_aspect` implementation (i3 "compatibility")
+
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
 - Deprecated [class_match](https://github.com/hyprland-community/pyprland/wiki/scratchpads_nonstandard) in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
 - Added [gbar](https://github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6
 - [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports multiple client windows (using 2.2.19 is recommended)
-- [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) and [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports rotation in 2.2.13
+- [monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) and [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports rotation in 2.2.13
 - Improve [Nix support](https://github.com/hyprland-community/pyprland/wiki/Nix)
 
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
```

### Comparing `pyprland-2.3.4/pyprland/adapters/menus.py` & `pyprland-2.3.5/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/adapters/units.py` & `pyprland-2.3.5/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/command.py` & `pyprland-2.3.5/pyprland/command.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/common.py` & `pyprland-2.3.5/pyprland/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,25 +33,32 @@
 
 DEBUG = os.environ.get("DEBUG", False)
 
 HYPRLAND_INSTANCE_SIGNATURE = os.environ.get("HYPRLAND_INSTANCE_SIGNATURE", "NO_INSTANCE")
 
 MINIMUM_ADDR_LEN = 4
 
+MAX_SOCKET_FILE_LEN = 15
+MAX_SOCKET_PATH_LEN = 108
+
 try:
+    # May throw an OSError because AF_UNIX path is too long: try to work around it only if needed
     original_ipc_folder = (
         f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}'
         if os.path.exists(f'{os.environ["XDG_RUNTIME_DIR"]}/hypr/{HYPRLAND_INSTANCE_SIGNATURE}')
         else f"/tmp/hypr/{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
     )
 
-    IPC_FOLDER = f"/tmp/.pypr-{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
-    # make a link from short path to original path
-    if not os.path.exists(IPC_FOLDER):
-        os.symlink(original_ipc_folder, IPC_FOLDER)
+    if len(original_ipc_folder) > MAX_SOCKET_PATH_LEN - MAX_SOCKET_FILE_LEN:
+        IPC_FOLDER = f"/tmp/.pypr-{HYPRLAND_INSTANCE_SIGNATURE}"  # noqa: S108
+        # make a link from short path to original path
+        if not os.path.exists(IPC_FOLDER):
+            os.symlink(original_ipc_folder, IPC_FOLDER)
+    else:
+        IPC_FOLDER = original_ipc_folder
 
 except KeyError:
     print("This is a fatal error, assuming we are running documentation generation or testing in a sandbox, hence ignoring it")
     IPC_FOLDER = "/"
 
 
 def set_terminal_size(descriptor: int, rows: int, cols: int) -> None:
```

### Comparing `pyprland-2.3.4/pyprland/ipc.py` & `pyprland-2.3.5/pyprland/ipc.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 import time
 from collections.abc import Callable, Iterable
 from functools import partial
 from logging import Logger
 from typing import Any, cast
 
 from .common import IPC_FOLDER, MINIMUM_ADDR_LEN, get_logger
-from .types import ClientInfo, MonitorInfo, PyprError
+from .types import ClientInfo, JSONResponse, MonitorInfo, PyprError, RetensionTimes
+from .utils import CacheData
 
 log: Logger | None = None
 
 HYPRCTL = f"{IPC_FOLDER}/.socket.sock"
 EVENTS = f"{IPC_FOLDER}/.socket2.sock"
 
 
@@ -38,14 +39,17 @@
 
 
 async def get_event_stream() -> tuple[asyncio.StreamReader, asyncio.StreamWriter]:
     """Return a new event socket connection."""
     return await asyncio.open_unix_connection(EVENTS)
 
 
+# Hyprctl JSON : cached responses {{{
+
+
 def retry_on_reset(func: Callable) -> Callable:
     """Retry on reset wrapper."""
 
     async def wrapper(*args, logger: Logger, **kwargs) -> Any:  # noqa: ANN401
         exc = None
         for count in range(3):
             try:
@@ -56,50 +60,63 @@
                 await asyncio.sleep(0.5 * count)
         logger.error("ipc connection failed.")
         raise ConnectionResetError from exc
 
     return wrapper
 
 
-cached_responses: dict[str, list[Any]] = {
-    # <command name>: [expiration_date, payload, retention_time]
-    "monitors": [0, None, 0.03],
-    # "workspaces": [0, None, 0.1],
-    # "clients": [0, None, 0.02],
+cached_responses: dict[str, CacheData] = {
+    # <command name>: CacheData
+    "monitors": CacheData(retension_time=RetensionTimes.LONG),
+    "workspaces": CacheData(retension_time=RetensionTimes.SHORT),
+    "clients": CacheData(retension_time=RetensionTimes.SHORT),
 }
 
 
+async def _get_response(command: bytes, logger: Logger) -> JSONResponse:
+    """Get response of `command` from the IPC socket."""
+    try:
+        reader, writer = await asyncio.open_unix_connection(HYPRCTL)
+    except FileNotFoundError as e:
+        logger.critical("hyprctl socket not found! is it running ?")
+        raise PyprError from e
+
+    writer.write(command)
+    await writer.drain()
+    reader_data = await reader.read()
+    writer.close()
+    await writer.wait_closed()
+    return json.loads(reader_data)  # type: ignore
+
+
 @retry_on_reset
-async def hyprctl_json(command: str, logger: Logger | None = None) -> list[dict[str, Any]] | dict[str, Any]:
+async def hyprctl_json(command: str, logger: Logger | None = None) -> JSONResponse:
     """Run an IPC command and return the JSON output."""
     logger = cast(Logger, logger or log)
     now = time.time()
-    cached = command in cached_responses and cached_responses[command][0] > now
-    if cached:
+    cache_data: CacheData | None = cached_responses.get(command)
+    if cache_data and cache_data.expiration_date > now:
         logger.debug("%s (CACHE HIT)", command)
-        return cached_responses[command][1]  # type: ignore
+        return await cache_data.wait_update()
+
     logger.debug(command)
-    try:
-        ctl_reader, ctl_writer = await asyncio.open_unix_connection(HYPRCTL)
-    except FileNotFoundError as e:
-        logger.critical("hyprctl socket not found! is it running ?")
-        raise PyprError from e
-    ctl_writer.write(f"-j/{command}".encode())
-    await ctl_writer.drain()
-    resp = await ctl_reader.read()
-    ctl_writer.close()
-    await ctl_writer.wait_closed()
-    ret = json.loads(resp)
+    if cache_data:  # should fill the cache
+        cache_data.set_pending(ref_time=now)
+
+    ret = await _get_response(f"-j/{command}".encode(), logger)
     assert isinstance(ret, list | dict)
-    if command in cached_responses:  # should fill the cache
-        cached_responses[command][0] = now + cached_responses[command][2]
-        cached_responses[command][1] = ret
+    if cache_data:
+        cache_data.set_value(ret)
     return ret
 
 
+# }}}
+
+
+# hyprctl : batched commands {{{
 def _format_command(command_list: list[str] | list[list[str]], default_base_command: str) -> Iterable[str]:
     """Format a list of commands to be sent to Hyprland.
 
     Args:
         command_list: list of commands to send
             Each command can be a string or a tuple with the command and the base command
         default_base_command: type of command to send
@@ -143,14 +160,17 @@
     await ctl_writer.wait_closed()
     r: bool = resp == b"ok" * nb_cmds
     if not r:
         logger.error("FAILED %s", resp)
     return r
 
 
+# }}}
+
+
 async def get_focused_monitor_props(logger: Logger | None = None, name: str | None = None) -> MonitorInfo:
     """Return focused monitor data if `name` is not defined, else use monitor's name.
 
     Args:
         logger: logger to use in case of error
         name: (optional) monitor name
```

### Comparing `pyprland-2.3.4/pyprland/plugins/expose.py` & `pyprland-2.3.5/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.3.5/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/gbar.py` & `pyprland-2.3.5/pyprland/plugins/gbar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Run gbar on the first available display from a list of displays."""
 
 import asyncio
 import contextlib
+from time import time
 
 from ..common import state
 from .interface import Plugin
 
 
 class Extension(Plugin):
     """Manage gBar application."""
@@ -16,18 +17,25 @@
 
     ongoing_task: asyncio.Task | None = None
 
     def _run_gbar(self, cmd: str) -> None:
         """Create ongoing task restarting gbar in case of crash."""
 
         async def _run_loop() -> None:
+            prev_time = time()
             while True:
                 self.proc = await asyncio.create_subprocess_shell(cmd)
                 await self.proc.wait()
-                self.notify_error("gBar crashed, restarting")
+                now = time()
+                delay = 5 - (now - prev_time)
+                text = f"gBar crashed, restarting in {delay:.1f}s." if delay > 0 else "gBar crashed, restarting."
+                await self.notify_error(f"gBar crashed, {text}")
+                prev_time = now
+                if delay > 0:
+                    await asyncio.sleep(delay)
 
         if self.ongoing_task:
             self.ongoing_task.cancel()
         self.ongoing_task = asyncio.create_task(_run_loop())
 
     async def run_gbar(self, args: str) -> None:
         """Start gBar on the first available monitor."""
```

### Comparing `pyprland-2.3.4/pyprland/plugins/interface.py` & `pyprland-2.3.5/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/layout_center.py` & `pyprland-2.3.5/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/lost_windows.py` & `pyprland-2.3.5/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/magnify.py` & `pyprland-2.3.5/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/monitors.py` & `pyprland-2.3.5/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/monitors_v0.py` & `pyprland-2.3.5/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/pyprland.py` & `pyprland-2.3.5/pyprland/plugins/pyprland.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Not a real Plugin - provides some core features and some caching of commonly requested structures."""
 
 import json
 
-from ..common import MINIMUM_ADDR_LEN, state
+from ..common import state
 from ..types import VersionInfo
 from .interface import Plugin
 
 DEFAULT_VERSION = VersionInfo(9, 9, 9)
 
 
 class Extension(Plugin):
@@ -64,16 +64,16 @@
         state.variables = self.config.get("variables", {})
         version_override = self.config.get("hyprland_version")
         if version_override:
             self.__set_hyprland_version(version_override)
 
     async def event_activewindowv2(self, addr: str) -> None:
         """Keep track of the focused client."""
-        if not addr or len(addr) < MINIMUM_ADDR_LEN:
-            self.log.warning("Active window is incorrect: %s.", addr)
+        if not addr:
+            self.log.debug("no active window")
             state.active_window = ""
         else:
             state.active_window = "0x" + addr
             self.log.debug("active_window = %s", state.active_window)
 
     async def event_workspace(self, workspace: str) -> None:
         """Track the active workspace."""
```

### Comparing `pyprland-2.3.4/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.3.5/pyprland/plugins/scratchpads/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,17 @@
         }
         await self.hyprctl(
             [f"{animation_actions[animation_type]},address:{addr}" for addr in addresses if animation_type in animation_actions]
         )
 
     async def run_show(self, uid: str) -> None:
         """<name> shows scratchpad "name"."""
+        if uid == "*":
+            await asyncio.gather(*(self.run_show(s.uid) for s in self.scratches.values() if not s.visible))
+            return
         scratch = self.scratches.get(uid)
 
         if not scratch:
             self.log.warning("%s doesn't exist, can't hide.", uid)
             await notify_error(f"Scratchpad '{uid}' not found, check your configuration or the show parameter")
             return
 
@@ -684,14 +687,17 @@
 
     async def run_hide(self, uid: str, force: bool = False, autohide: bool = False) -> None:
         """<name> hides scratchpad "name".
 
         if `autohide` is True, skips focus tracking
         `force` ignores the visibility check
         """
+        if uid == "*":
+            await asyncio.gather(*(self.run_hide(s.uid) for s in self.scratches.values() if s.visible))
+            return
         scratch = self.scratches.get(uid)
         active_window = state.active_window
         active_workspace = state.active_workspace
 
         if not scratch:
             await notify_error(f"Scratchpad '{uid}' not found, check your configuration or the hide parameter")
             self.log.warning("%s is not configured", uid)
```

### Comparing `pyprland-2.3.4/pyprland/plugins/scratchpads/animations.py` & `pyprland-2.3.5/pyprland/plugins/scratchpads/animations.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.3.5/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.3.5/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.3.5/pyprland/plugins/scratchpads/objects.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/shift_monitors.py` & `pyprland-2.3.5/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.3.5/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/system_notifier.py` & `pyprland-2.3.5/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/toggle_dpms.py` & `pyprland-2.3.5/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/toggle_special.py` & `pyprland-2.3.5/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/wallpapers.py` & `pyprland-2.3.5/pyprland/plugins/wallpapers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.3.5/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.3.4/pyprland/types.py` & `pyprland-2.3.5/pyprland/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """Common types from Hyprland API."""
 
 from dataclasses import dataclass
+from enum import Enum
 from typing import TypedDict
 
+PlainTypes = float | str | dict[str, "PlainTypes"] | list["PlainTypes"]
+JSONResponse = dict[str, PlainTypes] | list[dict[str, PlainTypes]]
+
+
+class RetensionTimes(float, Enum):
+    """Cache retension times."""
+
+    SHORT: float = 0.005
+    LONG: float = 0.05
+
 
 class WorkspaceDf(TypedDict):
     """Workspace definition."""
 
     id: int
     name: str
```

### Comparing `pyprland-2.3.4/pyproject.toml` & `pyprland-2.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyprland"
-version = "2.3.4"
+version = "2.3.5"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.3.4/PKG-INFO` & `pyprland-2.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.3.4
+Version: 2.3.5
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -80,21 +80,30 @@
 <details>
 <summary>
 Latest major changes
 </summary>
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
+### 2.3
+
+- Supports _Hyprland > 0.40.0_
+- Improved code kwaleetee
+- [monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) allows general monitor settings
+- [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
+  - better multi-window support
+  - better `preserve_aspect` implementation (i3 "compatibility")
+
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
 - Deprecated [class_match](https://github.com/hyprland-community/pyprland/wiki/scratchpads_nonstandard) in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
 - Added [gbar](https://github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6
 - [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports multiple client windows (using 2.2.19 is recommended)
-- [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) and [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports rotation in 2.2.13
+- [monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) and [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads) supports rotation in 2.2.13
 - Improve [Nix support](https://github.com/hyprland-community/pyprland/wiki/Nix)
 
 
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
```

