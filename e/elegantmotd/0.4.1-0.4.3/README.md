# Comparing `tmp/elegantmotd-0.4.1.tar.gz` & `tmp/elegantmotd-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elegantmotd-0.4.1.tar", max compression
+gzip compressed data, was "elegantmotd-0.4.3.tar", max compression
```

## Comparing `elegantmotd-0.4.1.tar` & `elegantmotd-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1563 2024-05-02 22:14:46.418129 elegantmotd-0.4.1/README.md
--rw-r--r--   0        0        0      760 2024-05-02 22:14:46.418129 elegantmotd-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/__init__.py
--rw-r--r--   0        0        0      103 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/__main__.py
--rw-r--r--   0        0        0      200 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/constants.py
--rw-r--r--   0        0        0      841 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/cpu.py
--rw-r--r--   0        0        0     1058 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/disk.py
--rw-r--r--   0        0        0      305 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/load.py
--rw-r--r--   0        0        0      376 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/loggedinusers.py
--rw-r--r--   0        0        0     1451 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/memory.py
--rw-r--r--   0        0        0     3206 2024-05-02 22:17:09.913423 elegantmotd-0.4.1/src/elegantmotd/motd.py
--rw-r--r--   0        0        0      553 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/network.py
--rw-r--r--   0        0        0      290 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/process.py
--rw-r--r--   0        0        0      286 2024-05-02 22:14:46.419129 elegantmotd-0.4.1/src/elegantmotd/sysinfo.py
--rw-r--r--   0        0        0     1436 2024-05-02 22:14:46.420128 elegantmotd-0.4.1/src/elegantmotd/temperature.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 elegantmotd-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1563 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/README.md
+-rw-r--r--   0        0        0      778 2024-05-30 11:48:11.539920 elegantmotd-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/__main__.py
+-rw-r--r--   0        0        0      200 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/constants.py
+-rw-r--r--   0        0        0      819 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/cpu.py
+-rw-r--r--   0        0        0     1036 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/disk.py
+-rw-r--r--   0        0        0      294 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/load.py
+-rw-r--r--   0        0        0      365 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/loggedinusers.py
+-rw-r--r--   0        0        0     1429 2024-05-30 11:44:38.637877 elegantmotd-0.4.3/src/elegantmotd/memory.py
+-rw-r--r--   0        0        0     2869 2024-05-30 11:44:38.638877 elegantmotd-0.4.3/src/elegantmotd/motd.py
+-rw-r--r--   0        0        0      542 2024-05-30 11:44:38.638877 elegantmotd-0.4.3/src/elegantmotd/network.py
+-rw-r--r--   0        0        0      279 2024-05-30 11:44:38.638877 elegantmotd-0.4.3/src/elegantmotd/process.py
+-rw-r--r--   0        0        0      286 2024-05-30 11:44:38.638877 elegantmotd-0.4.3/src/elegantmotd/sysinfo.py
+-rw-r--r--   0        0        0     1414 2024-05-30 11:44:38.638877 elegantmotd-0.4.3/src/elegantmotd/temperature.py
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 elegantmotd-0.4.3/PKG-INFO
```

### Comparing `elegantmotd-0.4.1/README.md` & `elegantmotd-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `elegantmotd-0.4.1/pyproject.toml` & `elegantmotd-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "elegantmotd"
-version = "0.4.1"
+version = "0.4.3"
 authors = ["Emerick Biron <emerick.biron@gmail.com>"]
 readme = "README.md"
 description = "A visually appealing and informative Message of the Day (MOTD) generator for Linux systems."
 homepage = "https://github.com/emerick-biron/elegantmotd"
 repository = "https://github.com/emerick-biron/elegantmotd.git"
 keywords = ["motd", "system", "information", "console", "dashboard"]
 license = "MIT"
 packages = [{ include = "elegantmotd", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-rich = "^13.3.4"
-psutil = "^5.9.5"
-art = "^5.9"
-rich-click = "^1.6.1"
+rich = "^13.7.1"
+psutil = "^5.9.8"
+art = "^6.2"
+rich-click = "^1.8.2"
+distro = "^1.9.0"
 
 [tool.poetry.scripts]
 elegantmotd="elegantmotd.motd:display"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/cpu.py` & `elegantmotd-0.4.3/src/elegantmotd/cpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 import psutil
 from rich.console import RenderableType
 from rich.progress import Progress, BarColumn, TaskProgressColumn
 
-from elegantmotd.constants import GREEN, RED, ORANGE, YELLOW
-from elegantmotd.sysinfo import SysInfo
+from .constants import GREEN, RED, ORANGE, YELLOW
+from .sysinfo import SysInfo
 
 
 class CPU(SysInfo):
     def _get_infos(self) -> Dict[RenderableType, RenderableType]:
         cpu_percent = psutil.cpu_percent()
         color = (
             GREEN if cpu_percent < 25
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/disk.py` & `elegantmotd-0.4.3/src/elegantmotd/disk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import shutil
 from typing import Dict
 
 from rich.console import RenderableType
 from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
 
-from elegantmotd.constants import GB, GREEN, YELLOW, ORANGE, RED
-from elegantmotd.sysinfo import SysInfo
+from .constants import GB, GREEN, YELLOW, ORANGE, RED
+from .sysinfo import SysInfo
 
 
 class Disk(SysInfo):
     def _get_infos(self) -> Dict[RenderableType, RenderableType]:
         disk_usage = shutil.disk_usage('/')
         total_space = f"{round(disk_usage.total / GB, 2)}GB"
         usage_percent = round((disk_usage.used / disk_usage.total * 100), 1)
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/memory.py` & `elegantmotd-0.4.3/src/elegantmotd/memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 import psutil
 from rich.console import RenderableType
 from rich.progress import Progress, BarColumn, TaskProgressColumn, TextColumn
 
-from elegantmotd.constants import GB, GREEN, YELLOW, ORANGE, RED
-from elegantmotd.sysinfo import SysInfo
+from .constants import GB, GREEN, YELLOW, ORANGE, RED
+from .sysinfo import SysInfo
 
 
 class Memory(SysInfo):
     def _get_infos(self) -> Dict[RenderableType, RenderableType]:
         memory_usage = psutil.virtual_memory()
         memory_progress, memory_usage_percent = self.__get_process(memory_usage)
         memory_progress.add_task("memory_progress", total=100, completed=round(memory_usage_percent))
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/motd.py` & `elegantmotd-0.4.3/src/elegantmotd/motd.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,37 +9,28 @@
 import rich_click as click
 from art import text2art
 from rich.console import Console
 from rich.live import Live
 from rich.padding import Padding
 from rich.style import Style
 from rich.table import Table
+import distro
 
-from elegantmotd.cpu import CPU
-from elegantmotd.disk import Disk
-from elegantmotd.load import Load
-from elegantmotd.loggedinusers import LoggedInUsers
-from elegantmotd.memory import Memory
-from elegantmotd.network import Network
-from elegantmotd.process import Process
-from elegantmotd.temperature import Temperature
+from .cpu import CPU
+from .disk import Disk
+from .load import Load
+from .loggedinusers import LoggedInUsers
+from .memory import Memory
+from .network import Network
+from .process import Process
+from .temperature import Temperature
 
 
 def get_distro_info():
-    try:
-        with open("/etc/lsb-release") as f:
-            content = f.read()
-        release_info = dict(re.findall(r'(\w+)=(.*)', content))
-        distro = f"{release_info['DISTRIB_ID']} {release_info['DISTRIB_RELEASE']}"
-        codename = release_info['DISTRIB_CODENAME']
-    except FileNotFoundError:
-        distro = "Unknown"
-        codename = "unknown"
-
-    return distro, codename
+    return f"{distro.id().capitalize()} {distro.version()} {distro.codename()}"
 
 
 def get_kernel_info():
     return platform.release()
 
 
 def get_architecture():
@@ -48,24 +39,25 @@
 
 @click.command(help="Display system information in a visually appealing manner.")
 @click.option("-w", "--watch", is_flag=True, show_default=False, default=False,
               help="Enable live updates of the system information.")
 def display(watch: bool) -> None:
     console = Console()
     try:
-        distro, codename = get_distro_info()
+        distro_info = get_distro_info()
         kernel = get_kernel_info()
         architecture = get_architecture()
 
         if watch:
             console.clear()
 
-        art_user = "\n".join(" " + line for line in text2art(getpass.getuser(), font='small').split("\n")[:-1])
-        
-        console.print(f"💻 [blue bold]{distro} {codename} LTS (GNU/Linux {kernel} {architecture}) [/]💻")
+        art_user = "\n".join(
+            " " + line for line in text2art(getpass.getuser(), font='small').split("\n")[:-1])
+
+        console.print(f"💻 [blue bold]{distro_info} LTS (GNU/Linux {kernel} {architecture}) [/]💻")
         console.print(f"[orange1 bold]{art_user}[/]")
         padding = Padding(generate_table(), (0, 0, 1, 0))
         if watch:
             with Live(padding, refresh_per_second=1) as live:
                 while True:
                     time.sleep(1)
                     padding.renderable = generate_table()
@@ -79,22 +71,27 @@
 def generate_table() -> Table:
     local_time = datetime.now(timezone.utc).astimezone()
     utc_offset = round(local_time.utcoffset().total_seconds() / 3600)
     table = Table(
         show_header=False,
         box=None,
         title_justify="left",
-        title=f" System information as of {local_time.strftime('%a. %d %B %Y %H:%M:%S')} UTC+{utc_offset}\n",
+        title=(
+            f" System information as of {local_time.strftime('%a. %d %B %Y %H:%M:%S')} "
+            f"UTC+{utc_offset}\n"
+        ),
         title_style=Style(color="white", italic=False, bold=True, ),
         expand=True,
         leading=1,
         padding=(0, 2)
     )
     table.add_column("Info", style="bold CYAN")
     table.add_column("Value", style="bold WHITE")
-    sysinfos = [Load(), Disk(), Memory(), Temperature(), Process(), LoggedInUsers(), Network(), CPU()]
-    [table.add_row(f"{info}:", sysinfo.infos[info]) for sysinfo in sysinfos for info in sysinfo.infos]
+    sysinfos = [Load(), Disk(), Memory(), Temperature(),
+                Process(), LoggedInUsers(), Network(), CPU()]
+    [table.add_row(f"{info}:", sysinfo.infos[info])
+     for sysinfo in sysinfos for info in sysinfo.infos]
     return table
 
 
 if __name__ == '__main__':
     display(sys.argv[1:])
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/network.py` & `elegantmotd-0.4.3/src/elegantmotd/network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from socket import AF_INET
 from typing import Dict
 
 import psutil
 from rich.console import RenderableType
 
-from elegantmotd.sysinfo import SysInfo
+from .sysinfo import SysInfo
 
 
 class Network(SysInfo):
     def _get_infos(self) -> Dict[RenderableType, RenderableType]:
         infos = {"Network": ""}
 
         addrs = psutil.net_if_addrs()
```

### Comparing `elegantmotd-0.4.1/src/elegantmotd/temperature.py` & `elegantmotd-0.4.3/src/elegantmotd/temperature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Union
 
 import psutil
 from rich.console import RenderableType
 from rich.text import Text
 
-from elegantmotd.constants import GREEN, YELLOW, ORANGE, RED
-from elegantmotd.sysinfo import SysInfo
+from .constants import GREEN, YELLOW, ORANGE, RED
+from .sysinfo import SysInfo
 
 
 class Temperature(SysInfo):
     def _get_infos(self) -> Dict[RenderableType, RenderableType]:
         infos = {"Temperature": ""}
         temp_info = psutil.sensors_temperatures()
         if "coretemp" in temp_info:
```

### Comparing `elegantmotd-0.4.1/PKG-INFO` & `elegantmotd-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: elegantmotd
-Version: 0.4.1
+Version: 0.4.3
 Summary: A visually appealing and informative Message of the Day (MOTD) generator for Linux systems.
 Home-page: https://github.com/emerick-biron/elegantmotd
 License: MIT
 Keywords: motd,system,information,console,dashboard
 Author: Emerick Biron
 Author-email: emerick.biron@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: art (>=5.9,<6.0)
-Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
-Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Requires-Dist: art (>=6.2,<7.0)
+Requires-Dist: distro (>=1.9.0,<2.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: rich-click (>=1.8.2,<2.0.0)
 Project-URL: Repository, https://github.com/emerick-biron/elegantmotd.git
 Description-Content-Type: text/markdown
 
 # ElegantMOTD
 
 ElegantMOTD is a Python-based Message of the Day (MOTD) generator for displaying system information in a visually
 appealing and informative manner. It works on Linux systems and provides details such as system load, disk usage, memory
```

