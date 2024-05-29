# Comparing `tmp/systembridgedata-5.0.0.dev0.tar.gz` & `tmp/systembridgedata-5.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgedata-5.0.0.dev0.tar", last modified: Wed May 29 21:38:50 2024, max compression
+gzip compressed data, was "systembridgedata-5.0.0.dev1.tar", last modified: Wed May 29 22:18:02 2024, max compression
```

## Comparing `systembridgedata-5.0.0.dev0.tar` & `systembridgedata-5.0.0.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/systembridgedata/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/systembridgedata/module/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/systembridgedata/module/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 21:38:50.000000 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 21:38:50.000000 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:38:50.000000 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:38:50.000000 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 21:38:50.000000 systembridgedata-5.0.0.dev0/systembridgedata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:38:50.734773 systembridgedata-5.0.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 21:38:28.000000 systembridgedata-5.0.0.dev0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.244769 systembridgedata-5.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:18:02.244769 systembridgedata-5.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata/module/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/tests/test_version.py
```

### Comparing `systembridgedata-5.0.0.dev0/LICENSE` & `systembridgedata-5.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev0/PKG-INFO` & `systembridgedata-5.0.0.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgedata
-Version: 5.0.0.dev0
+Version: 5.0.0.dev1
 Summary: System Bridge Data
 Home-page: https://github.com/timmo001/system-bridge-data
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgedata-5.0.0.dev0/pyproject.toml` & `systembridgedata-5.0.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev0/setup.py` & `systembridgedata-5.0.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/cpu.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/cpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         """Initialise."""
         super().__init__()
 
         self._count: int = cpu_count()
 
         self.sensors: Sensors | None = None
 
-    async def get_frequency(self) -> scpufreq:
+    def get_frequency(self) -> scpufreq:
         """CPU frequency."""
         return cpu_freq()
 
-    async def get_frequency_per_cpu(
+    def get_frequency_per_cpu(
         self,
     ) -> list[scpufreq]:
         """CPU frequency per CPU."""
         return cpu_freq(percpu=True)  # type: ignore
 
-    async def get_load_average(self) -> float:
+    def get_load_average(self) -> float:
         """Get load average."""
         avg_tuple = getloadavg()
         return sum([avg_tuple[0], avg_tuple[1], avg_tuple[2]]) / 3
 
-    async def get_power_package(self) -> float | None:
+    def get_power_package(self) -> float | None:
         """CPU package power."""
         if (
             self.sensors is None
             or self.sensors.windows_sensors is None
             or self.sensors.windows_sensors.hardware is None
         ):
             return None
@@ -66,15 +66,15 @@
                     return (
                         float(sensor.value)
                         if isinstance(sensor.value, (int, float))
                         else None
                     )
         return None
 
-    async def get_power_per_cpu(self) -> list[float] | None:
+    def get_power_per_cpu(self) -> list[float] | None:
         """CPU package power."""
         powers: list[float] = [-1] * self._count
         if (
             self.sensors is None
             or self.sensors.windows_sensors is None
             or self.sensors.windows_sensors.hardware is None
         ):
@@ -110,19 +110,19 @@
                                 sensor.value,
                             )
                             index = int(sensor.id.split("/")[-1])
                             powers[index] = float(sensor.value)
 
         return powers
 
-    async def get_stats(self) -> scpustats:
+    def get_stats(self) -> scpustats:
         """CPU stats."""
         return cpu_stats()
 
-    async def get_temperature(self) -> float | None:
+    def get_temperature(self) -> float | None:
         """CPU temperature."""
         if self.sensors is not None:
             if self.sensors.temperatures is not None:
                 temperatures: dict[str, list[shwtemp]] = self.sensors.temperatures
                 if "k10temp" in temperatures:
                     for sensor in self.sensors.temperatures["k10temp"]:
                         self._logger.debug("k10temp: %s", sensor)
@@ -185,45 +185,45 @@
                             return (
                                 float(sensor.value)
                                 if isinstance(sensor.value, (int, float, str))
                                 else None
                             )
         return None
 
-    async def get_times(self) -> pcputimes:
+    def get_times(self) -> pcputimes:
         """CPU times."""
         return cpu_times(percpu=False)
 
-    async def get_times_percent(self) -> pcputimes:
+    def get_times_percent(self) -> pcputimes:
         """CPU times percent."""
         return cpu_times_percent(interval=1, percpu=False)
 
-    async def get_times_per_cpu(
+    def get_times_per_cpu(
         self,
     ) -> list[pcputimes]:
         """CPU times per CPU."""
         return cpu_times(percpu=True)
 
-    async def get_times_per_cpu_percent(
+    def get_times_per_cpu_percent(
         self,
     ) -> list[pcputimes]:
         """CPU times per CPU percent."""
         return cpu_times_percent(interval=1, percpu=True)
 
-    async def get_usage(self) -> float:
+    def get_usage(self) -> float:
         """CPU usage."""
         return cpu_percent(interval=1, percpu=False)
 
-    async def get_usage_per_cpu(
+    def get_usage_per_cpu(
         self,
     ) -> list[float]:
         """CPU usage per CPU."""
         return cpu_percent(interval=1, percpu=True)  # type: ignore
 
-    async def get_voltages(self) -> tuple[float | None, list[float]]:
+    def get_voltages(self) -> tuple[float | None, list[float]]:
         """CPU voltage."""
         voltage: float | None = None
         voltages: list[float] = [-1] * self._count
         voltage_sensors = []
         if (
             self.sensors is None
             or self.sensors.windows_sensors is None
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/disks.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/disks.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from systembridgeshared.base import Base
 
 
 class Disks(Base):
     """Disks data."""
 
-    async def get_io_counters(self) -> sdiskio | None:
+    def get_io_counters(self) -> sdiskio | None:
         """Disk IO counters."""
         return disk_io_counters()
 
-    async def get_io_counters_per_disk(self) -> dict[str, sdiskio]:
+    def get_io_counters_per_disk(self) -> dict[str, sdiskio]:
         """Disk IO counters per disk."""
         return disk_io_counters(perdisk=True)
 
-    async def get_partitions(self) -> list[sdiskpart]:
+    def get_partitions(self) -> list[sdiskpart]:
         """Disk partitions."""
         return disk_partitions(all=True)
 
-    async def get_usage(self, path: str) -> sdiskusage | None:
+    def get_usage(self, path: str) -> sdiskusage | None:
         """Disk usage."""
         try:
             return disk_usage(path)
         except (FileNotFoundError, PermissionError) as error:
             self._logger.warning(
                 "Error getting disk usage for: %s",
                 path,
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/media.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/media.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/networks.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/networks.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from systembridgeshared.base import Base
 
 
 class Networks(Base):
     """Networks data."""
 
-    async def get_addresses(
+    def get_addresses(
         self,
     ) -> dict[str, list[snicaddr]]:
         """Addresses."""
         return net_if_addrs()
 
-    async def get_connections(self) -> list[sconn]:
+    def get_connections(self) -> list[sconn]:
         """Get connections."""
         return net_connections("all")
 
-    async def get_io_counters(self) -> snetio:
+    def get_io_counters(self) -> snetio:
         """IO Counters."""
         return net_io_counters()
 
-    async def get_stats(self) -> dict[str, snicstats]:
+    def get_stats(self) -> dict[str, snicstats]:
         """Stats."""
         return net_if_stats()
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/processes.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/sensors.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 from systembridgeshared.base import Base
 
 
 class Sensors(Base):
     """Sensors data."""
 
-    async def get_fans(self) -> dict[str, list[sfan]] | None:
+    def get_fans(self) -> dict[str, list[sfan]] | None:
         """Get fans."""
         if not hasattr(psutil, "sensors_fans"):
             return None
         return psutil.sensors_fans()  # type: ignore
 
-    async def get_temperatures(self) -> dict[str, list[shwtemp]] | None:
+    def get_temperatures(self) -> dict[str, list[shwtemp]] | None:
         """Get temperatures."""
         if not hasattr(psutil, "sensors_temperatures"):
             return None
         return psutil.sensors_temperatures(fahrenheit=False)  # type: ignore
 
-    async def get_windows_sensors(self) -> dict | None:
+    def get_windows_sensors(self) -> dict | None:
         """Get windows sensors."""
         if sys.platform != "win32":
             return None
 
         try:
             # Import here to not raise error when importing file on linux
             # pylint: disable=import-error, import-outside-toplevel
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata/module/system.py` & `systembridgedata-5.0.0.dev1/systembridgedata/module/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,27 +62,27 @@
         # Determine the latest version URL based on the run mode
         self._version_latest_url = f"https://github.com/timmo001/{(
             'system-bridge' if self._run_mode == RunMode.STANDALONE else 'system-bridge-backend'
         )}/releases/latest"
 
         self._version_latest: str | None = None
 
-    async def get_active_user_id(self) -> int:
+    def get_active_user_id(self) -> int:
         """Get active user ID."""
         return os.getpid()
 
-    async def get_active_user_name(self) -> str | None:
+    def get_active_user_name(self) -> str | None:
         """Get active user."""
         return getpass.getuser()
 
-    async def get_boot_time(self) -> float:
+    def get_boot_time(self) -> float:
         """Get boot time."""
         return boot_time()
 
-    async def get_camera_usage(self) -> list[str]:
+    def get_camera_usage(self) -> list[str]:
         """Return a list of apps that are currently using the webcam."""
         active_apps: list[str] = []
         if sys.platform == "win32":
             # Read from registry for camera usage
             import winreg  # pylint: disable=import-error,import-outside-toplevel
 
             subkey_path = r"SOFTWARE\Microsoft\Windows\CurrentVersion\CapabilityAccessManager\ConsentStore\webcam"
@@ -126,45 +126,45 @@
             except OSError:
                 pass
         elif sys.platform in ["darwin", "linux"]:
             # Unknown, please open an issue or PR if you know how to do this
             pass
         return active_apps
 
-    async def get_fqdn(self) -> str:
+    def get_fqdn(self) -> str:
         """Get FQDN."""
         return socket.getfqdn()
 
-    async def get_hostname(self) -> str:
+    def get_hostname(self) -> str:
         """Get hostname."""
         return socket.gethostname()
 
-    async def get_ip_address_4(self) -> str:
+    def get_ip_address_4(self) -> str:
         """Get IPv4 address."""
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             sock.connect(("8.8.8.8", 80))
             return sock.getsockname()[0]
         except OSError:
             return ""
 
-    async def get_ip_address_6(self) -> str:
+    def get_ip_address_6(self) -> str:
         """Get IPv6 address."""
         try:
             sock = socket.socket(socket.AF_INET6, socket.SOCK_DGRAM)
             sock.connect(("2001:4860:4860::8888", 80))
             return sock.getsockname()[0]
         except OSError:
             return ""
 
     def get_mac_address(self) -> str:
         """Get MAC address."""
         return ":".join(re.findall("..", f"{uuid.getnode():012x}"))
 
-    async def get_pending_reboot(self) -> bool:
+    def get_pending_reboot(self) -> bool:
         """Check if there is a pending reboot."""
         if sys.platform == "win32":
             # Read from registry for pending reboot
             import winreg  # pylint: disable=import-error,import-outside-toplevel
 
             reg = winreg.ConnectRegistry(None, winreg.HKEY_LOCAL_MACHINE)
             # Check for "Reboot Required" keys
@@ -221,27 +221,27 @@
         elif sys.platform in ["darwin", "linux"]:
             if os.path.exists("/var/run/reboot-required"):
                 return True
             if os.path.exists("/var/run/reboot-required.pkgs"):
                 return True
         return False
 
-    async def get_platform(self) -> str:
+    def get_platform(self) -> str:
         """Get platform."""
         return platform.system()
 
-    async def get_platform_version(self) -> str:
+    def get_platform_version(self) -> str:
         """Get platform version."""
         return platform.version()
 
-    async def get_uptime(self) -> float:
+    def get_uptime(self) -> float:
         """Get uptime."""
         return os.times().system
 
-    async def get_users(self) -> list[suser]:  # pylint: disable=unsubscriptable-object
+    def get_users(self) -> list[suser]:  # pylint: disable=unsubscriptable-object
         """Get users."""
         return users()
 
     @property
     def _uuid(self) -> str:
         """Get UUID."""
         # cat /var/lib/dbus/machine-id
@@ -293,12 +293,12 @@
                 data = await response.json()
                 if data is not None and (tag_name := data.get("tag_name")) is not None:
                     self._version_latest = tag_name.replace("v", "")
                     self._logger.info("Latest version: %s", self._version_latest)
 
         return self._version_latest
 
-    async def get_version_newer_available(self) -> bool | None:
+    def get_version_newer_available(self) -> bool | None:
         """Check if newer version is available."""
         if self._version_latest is not None and self._version is not None:
             return parse(self._version_latest) > parse(self._version)
         return None
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata.egg-info/PKG-INFO` & `systembridgedata-5.0.0.dev1/systembridgedata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgedata
-Version: 5.0.0.dev0
+Version: 5.0.0.dev1
 Summary: System Bridge Data
 Home-page: https://github.com/timmo001/system-bridge-data
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgedata-5.0.0.dev0/systembridgedata.egg-info/SOURCES.txt` & `systembridgedata-5.0.0.dev1/systembridgedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

