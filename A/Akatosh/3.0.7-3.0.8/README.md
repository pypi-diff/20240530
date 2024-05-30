# Comparing `tmp/akatosh-3.0.7.tar.gz` & `tmp/akatosh-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.7.tar", max compression
+gzip compressed data, was "akatosh-3.0.8.tar", max compression
```

## Comparing `akatosh-3.0.7.tar` & `akatosh-3.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      544 2024-05-08 01:04:21.582527 akatosh-3.0.7/Akatosh/__init__.py
--rw-r--r--   0        0        0     5333 2024-05-08 01:04:21.583527 akatosh-3.0.7/Akatosh/entity.py
--rw-r--r--   0        0        0     6375 2024-05-17 03:52:58.399245 akatosh-3.0.7/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.7/Akatosh/resource.py
--rw-r--r--   0        0        0     6109 2024-05-17 03:56:22.573448 akatosh-3.0.7/Akatosh/universe.py
--rw-r--r--   0        0        0      321 2024-05-17 03:56:29.523927 akatosh-3.0.7/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.7/README.md
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0      544 2024-05-08 01:04:21.582527 akatosh-3.0.8/Akatosh/__init__.py
+-rw-r--r--   0        0        0     5333 2024-05-08 01:04:21.583527 akatosh-3.0.8/Akatosh/entity.py
+-rw-r--r--   0        0        0     6724 2024-05-30 05:04:43.290585 akatosh-3.0.8/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.8/Akatosh/resource.py
+-rw-r--r--   0        0        0     6389 2024-05-30 04:56:21.823830 akatosh-3.0.8/Akatosh/universe.py
+-rw-r--r--   0        0        0      321 2024-05-30 05:06:06.573059 akatosh-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.8/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.8/PKG-INFO
```

### Comparing `akatosh-3.0.7/Akatosh/__init__.py` & `akatosh-3.0.8/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.7/Akatosh/entity.py` & `akatosh-3.0.8/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.7/Akatosh/event.py` & `akatosh-3.0.8/Akatosh/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,16 +79,24 @@
                 and self.next <= Mundus.time
             ):
                 if asyncio.iscoroutinefunction(self._action):
                     await self._action()
                 else:
                     self._action()
                 self._acted = True
-                self._next += max(Mundus.time_step, self.step)
-                self._next = round(self._next, Mundus.time_resolution)
+                if Mundus.realtime:
+                    if self.step != Mundus.time_step:
+                        self._next = round(
+                            Mundus.time + self.step, Mundus.time_resolution
+                        )
+                    else:
+                        self._next = Mundus.time
+                else:
+                    self._next += max(Mundus.time_step, self.step)
+                    self._next = round(self._next, Mundus.time_resolution)
                 logger.debug(f"Event {self} acted at {Mundus.time}.")
                 if self._once == True:
                     self._ended = True
                     logger.debug(f"Event {self} ended at {Mundus.time}.")
                     return
 
             if self.ended == False:
```

### Comparing `akatosh-3.0.7/Akatosh/resource.py` & `akatosh-3.0.8/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.7/Akatosh/universe.py` & `akatosh-3.0.8/Akatosh/universe.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         if cls._instance is None:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self) -> None:
         """The simulation universe."""
         self._time_resolution = 3
+        self._time_scale = 1
         self._time_step = round(1 / pow(10, self.time_resolution), self.time_resolution)
         self._time = 0
         self._simulation_start_time = 0
         self._simulation_end_time = 0
         self._realtime = False
         self._current_event_priority = 0
         self._max_event_priority = 0
@@ -55,15 +56,15 @@
                         await asyncio.sleep(0)
                         self._current_event_priority += 1
                     # finish the iteration
                     iteration_end_time = time.perf_counter() - self.simulation_start_time
                     logger.debug(f"Iteration finished at Real Time: {iteration_end_time:0.6f}")
                     logger.debug(f"FPS: {1/(iteration_end_time - iteration_start_time):0.6f}")
                     # update the time
-                    self._time = time.perf_counter() - self.simulation_start_time
+                    self._time = (time.perf_counter() - self.simulation_start_time) * self.time_scale
                     await asyncio.sleep(0)
                     
                 else:
                     # iterate through all event priorities
                     self._current_event_priority = 0
                     while self.current_event_priority <= self._max_event_priority:
                         logger.debug(
@@ -80,18 +81,19 @@
             if self.realtime:
                 logger.info(
                     f"Simulation completed in {round(self.simulation_end_time - self.simulation_start_time, 6)} seconds, exceeding real time by {round(((self.simulation_end_time - self.simulation_start_time - till)/till)*100,2)}%."
                 )
 
         return time_flow()
 
-    def enable_realtime(self, time_resolution: int = 3):
+    def enable_realtime(self, time_resolution: int = 3, time_scale: float = 1):
         """Enable the real time simulation. Time step will be adjusted to 0.1s."""
         self.time_resolution = time_resolution
         self._time_step = round(1 / pow(10, self.time_resolution), self.time_resolution)
+        self._time_scale = time_scale
         self._realtime = True
 
     def set_logging_level(self, level: int = logging.DEBUG):
         """Set the logging level. Default is DEBUG."""
         logger.setLevel(level)
 
     @property
@@ -145,9 +147,13 @@
         return self._simulation_start_time
 
     @property
     def simulation_end_time(self):
         """The time when the simulation ended."""
         return self._simulation_end_time
 
+    @property
+    def time_scale(self):
+        """The time scale of the simulation. Default is 1. Only works in real time mode."""
+        return self._time_scale
 
 Mundus = Universe()
```

### Comparing `akatosh-3.0.7/README.md` & `akatosh-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.7/PKG-INFO` & `akatosh-3.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 3.0.7
+Version: 3.0.8
 Summary: 
 Author: Innovation Central Perth Maintainer
 Author-email: ryf0510@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

