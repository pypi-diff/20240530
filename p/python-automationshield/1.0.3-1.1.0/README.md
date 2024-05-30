# Comparing `tmp/python_automationshield-1.0.3.tar.gz` & `tmp/python_automationshield-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_automationshield-1.0.3.tar", max compression
+gzip compressed data, was "python_automationshield-1.1.0.tar", max compression
```

## Comparing `python_automationshield-1.0.3.tar` & `python_automationshield-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-25 13:39:55.334700 python_automationshield-1.0.3/LICENSE
--rw-r--r--   0        0        0     4590 2024-04-25 13:39:55.334700 python_automationshield-1.0.3/README.md
--rw-r--r--   0        0        0      752 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      655 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/__init__.py
--rw-r--r--   0        0        0     4473 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino.py
--rw-r--r--   0        0        0      113 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
--rw-r--r--   0        0        0      115 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/floatshield/floatshield.ino
--rw-r--r--   0        0        0      418 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
--rw-r--r--   0        0        0      447 2024-04-25 13:39:55.335700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
--rw-r--r--   0        0        0     2481 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
--rw-r--r--   0        0        0      986 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
--rw-r--r--   0        0        0      356 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
--rw-r--r--   0        0        0      367 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
--rw-r--r--   0        0        0      122 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
--rw-r--r--   0        0        0      269 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
--rw-r--r--   0        0        0      119 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
--rw-r--r--   0        0        0     7525 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/controller.py
--rw-r--r--   0        0        0       52 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/exception.py
--rw-r--r--   0        0        0       67 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/live_plotter.py
--rw-r--r--   0        0        0     1615 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/plotting/plotter.py
--rw-r--r--   0        0        0      186 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/aeroshield.py
--rw-r--r--   0        0        0    11947 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/baseshield.py
--rw-r--r--   0        0        0      468 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/dummyshield.py
--rw-r--r--   0        0        0     1060 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/floatshield.py
--rw-r--r--   0        0        0     6892 2024-04-25 13:39:55.336700 python_automationshield-1.0.3/src/automationshield/shields/magnetoshield.py
--rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-30 14:40:47.235680 python_automationshield-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4590 2024-05-30 14:40:47.235680 python_automationshield-1.1.0/README.md
+-rw-r--r--   0        0        0      812 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/__init__.py
+-rw-r--r--   0        0        0     4473 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino.py
+-rw-r--r--   0        0        0      113 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
+-rw-r--r--   0        0        0      115 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/floatshield/floatshield.ino
+-rw-r--r--   0        0        0      418 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
+-rw-r--r--   0        0        0      447 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
+-rw-r--r--   0        0        0     2481 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
+-rw-r--r--   0        0        0      986 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
+-rw-r--r--   0        0        0      356 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
+-rw-r--r--   0        0        0      367 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
+-rw-r--r--   0        0        0      122 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
+-rw-r--r--   0        0        0      269 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
+-rw-r--r--   0        0        0      119 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
+-rw-r--r--   0        0        0       73 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/controller/__init__.py
+-rw-r--r--   0        0        0     9561 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/controller/controller.py
+-rw-r--r--   0        0        0     1037 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/controller/reference.py
+-rw-r--r--   0        0        0       52 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/exception.py
+-rw-r--r--   0        0        0       67 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/__init__.py
+-rw-r--r--   0        0        0     6523 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/live_plotter.py
+-rw-r--r--   0        0        0     7716 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/plotter.py
+-rw-r--r--   0        0        0      187 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/__init__.py
+-rw-r--r--   0        0        0      840 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/_dummyshield.py
+-rw-r--r--   0        0        0     1973 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/aeroshield.py
+-rw-r--r--   0        0        0    11517 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/baseshield.py
+-rw-r--r--   0        0        0     1189 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/floatshield.py
+-rw-r--r--   0        0        0     6620 2024-05-30 14:40:47.240680 python_automationshield-1.1.0/src/automationshield/shields/magnetoshield.py
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 python_automationshield-1.1.0/PKG-INFO
```

### Comparing `python_automationshield-1.0.3/LICENSE` & `python_automationshield-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.3/README.md` & `python_automationshield-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.3/pyproject.toml` & `python_automationshield-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-automationshield"
-version = "1.0.3"
+version = "1.1.0"
 description = "A Python interface to AutomationShield's Arduino shields"
 authors = ["Bert Van den Abbeele"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/mrtreasurer/python-automationshield"
 documentation = "https://python-automationshield.readthedocs.io"
 packages = [
@@ -12,18 +12,20 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 matplotlib = ">=3.8.2"
 numpy = ">=1.26.3"
 pyserial = ">=3.5"
+multiprocess = ">=0.70.16"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
-sphinx-autoapi = "^3.0.0"
-myst-nb = "^1.0.0"
-sphinx-rtd-theme = "^2.0.0"
+sphinx-autoapi = ">=3.0.0"
+myst-nb = ">=1.0.0"
+sphinx-rtd-theme = ">=2.0.0"
+sphinx-copybutton = ">=0.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_automationshield-1.0.3/src/automationshield/__init__.py` & `python_automationshield-1.1.0/src/automationshield/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from .controller import ShieldController
 from .exception import AutomationShieldException
 from .shields import AeroShield, FloatShield, MagnetoShield, DummyShield
 
 
+# install arduino-cli if not present
 import platform
 
-from pathlib import Path
-
-from .arduino import download_cli, setup_cli, cli_dir, cli_path
+from .arduino import download_cli, setup_cli, cli_dir
 
 system = platform.system()
 
 if system in ("Windows", "Linux", "Darwin"):
     if not cli_dir.exists():
         print(f"Downloading arduino-cli to {cli_dir}")
         download_cli(system)
```

### Comparing `python_automationshield-1.0.3/src/automationshield/arduino.py` & `python_automationshield-1.1.0/src/automationshield/arduino.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp` & `python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.3/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h` & `python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.0.3/src/automationshield/controller.py` & `python_automationshield-1.1.0/src/automationshield/controller/controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,92 @@
+import ctypes
 import numpy as np
 import numpy.typing as npt
 import time
 
-from typing import Optional, Iterable
-
-from .shields.baseshield import BaseShield
-from .plotting import LivePlotter
+from multiprocess import Process, RawValue
+from multiprocess.shared_memory import SharedMemory
+from typing import Callable, Optional, Sequence, Type
+
+from .reference import Reference, ConstantReference, PresetReference
+
+from ..exception import AutomationShieldException
+from ..shields.baseshield import BaseShield
+from ..plotting import LivePlotter
 
 
 class ShieldController:
     """The ShieldController class implements a controller interface for the various shield classes. This class should be subclassed to create custom controllers.\
         In a subclass, overwrite the :py:meth:`ShieldController.controller` method to implement your controller. Optionally, overwrite the :py:meth:`ShieldController.variables` method \
         to initialise instance variables that should persist beyond the scope of the controller method.
 
     Example:
 
     >>> class MyController(ShieldController):
     ...     def controller(self, t: float, dt: float, ref: float, pot: float, sensor: float) -> float:
     ...         return ref
-
-    :param shield: shield class instance.
-    :type shield: ~automationshield.shields.BaseShield
-    :param n_base_vars: Number of variables that is saved by default. These are the time, reference, potentiometer, sensor and actuator values.
-    :type n_base_vars: int
-    :param tracked_variables: Mapping of additional variables to track during run.
-    :type tracked_variables: dict[str, int]
     """
     def __init__(self, shield:BaseShield) -> None:
+        """
+        :param shield: shield class instance.
+        :type shield: ~automationshield.shields.BaseShield
+        """
         self.shield = shield
 
+        # t1 - tstart, ref, pot, sensor, actuator
         self.n_base_vars = 5
         # store additional variables to save when running an experiment
         self.tracked_variables: dict[str, int] = dict()
 
         # initiate controller variables
         self.variables()
 
+        self.cntr = 0
+
     def variables(self) -> None:
         """Define variables to be used by the controller or saved during the experiment."""
         pass
 
-    def add_tracked_variable(self, name:str, size: Optional[int]=1) -> dict[str, int]:
+    def add_tracked_variable(self, name: str, size: int=1) -> dict[str, int]:
         """Add a variable to the list of variables whose value should be tracked during the experiment and returned afterwards.
         Variables should be instance variables of the class, otherwise they won't be accessible!
 
         :param name: Name of the variable, without 'self.'
         :type name: str
         :param size: Size of the variable, e.g. 3 for a three-dimensional position vector. Defaults to 1, i.e. single values.
-        :type size: int, optional
+        :type size: int
         :return: A copy of the current map of tracked variables and their respective size.
         :rtype: dict[str, int]
         """
         self.tracked_variables[name] = size
 
         return self.tracked_variables.copy()
 
-    def controller(self, t: float, dt: float, ref: float, pot: float, sensor: float) -> float:
+    def reference_callback(self, cntr: int, t: float, pot: float) -> int | float:
+        """Calculate reference value. If used, this method is called every cycle to calculate a new reference. After implementing this method on a subclass of :py:class:`ShieldController`, \
+            you can use it during an experiment as follows:
+
+        >>> my_controller = MyController(shield=shield)
+        >>> my_controller.run(freq=freq, cycles=cycles, ref=my_controller.reference_callback)
+
+        This implementation allows for multiple callback functions to be defined on the controller class or outside of it. It is not mandatory to override this specific method.
+
+        :param cntr: Number of the current cycle.
+        :type cntr: int
+        :param t: Time since start of experiment in seconds.
+        :type t: float
+        :param pot: Potentiometer value in percent.
+        :type pot: float
+        :return: Reference value.
+        :rtype: float
+        """
+
+        return 0
+
+    def controller(self, t: float, dt: float, ref: int | float, pot: float, sensor: float) -> int | float:
         """Implement the controller here. You can subclass ShieldController and overwrite the controller.
 
         :param t: Time since start of run in seconds.
         :type t: float
         :param dt: Length of current time step in seconds.
         :type dt: float
         :param ref: Reference value for the current step.
@@ -70,110 +97,120 @@
         :type sensor: float
         :return: input value for actuator. the motor value will be saturated afterwards.
         :rtype: float
         """
 
         return 0  # actuator value
 
-    def run(self, freq: int, cycles: int, ref: Optional[float | int | Iterable[float|int]]=None, live_plotter: Optional[LivePlotter]=None) -> npt.NDArray[np.float_]:
+    def run(self, freq: int | float, cycles: Optional[int]=None, ref: Optional[int | float | Sequence[int | float] | Callable[[int, float, float], int | float] | Reference]=None, live_plotter: Optional[LivePlotter]=None) -> npt.NDArray[np.float64]:
         """Run the controller on a shield device.
 
         :param freq: Desired frequency of the loop.
         :type freq: int
-        :param cycles: Number of cycles to run the experiment.
+        :param cycles: Number of cycles to run the experiment. If ref is an array, cycles is optional and the length of the reference is used as the number of cycles. Defaults to None.
         :type cycles: int
-        :param ref: The reference to follow. It should have a lenght equal to freq * time or be a single value for a constant reference. Defaults to None, in which case the reference is set to 0.
-        :type ref: Optional[float  |  int  |  Iterable[float | int]], optional
+        :param ref: The reference to follow. It can be an array, a single value (i.e. constant reference) or a function or class to be called in each cycle. \
+            If it's an array, it should have a length equal to freq * cycles. See the documentation for :py:meth:`ShieldController.reference_callback` on how to define a callback function. \
+            A class should expose a :py:meth:`__call__` method, whose signature must match that of a callback function, like in ~automationshield.controller.Reference. \
+            The class doesn't need to inherit from ~automationshield.controller.reference. Defaults to None, in which case the reference is set to 0.
+        :type ref: float | int | Sequence[float | int] | Callable[[int, float, float], float], Type[~automationshield.controller.Reference], optional
         :param live_plotter: Optional :py:class:`~automationshield.plotting.LivePlotter` instance to use for displaying a live plot, defaults to None.
         :type live_plotter: ~automationshield.plotting.LivePlotter, optional
         :return: Experiment data. The columns of the array are time, reference, potentiometer, sensor, actuator, and any additional variables in the order they were added.
-        :rtype: npt.NDArray[np.float\_]
+        :rtype: npt.NDArray[np.float64]
         """
 
-        cntr = 0
-        maxcntr = cycles
-        period = 1/freq
+        # if cycles is given, use that. Otherwise, check if ref has a length.
+        if cycles is None:
+            if hasattr(ref, "__len__"):
+                cycles = len(ref)
+            else:
+                raise AutomationShieldException("Cycles must be given or ref should be sequence")
+
+        if callable(ref):
+            pass
+        elif ref is None:
+            ref = ConstantReference(0)
+        elif isinstance(ref, (int, float)):
+            ref = ConstantReference(ref)
+        elif hasattr(ref, "__getitem__"):
+            ref = PresetReference(ref)
+        else:
+            raise TypeError(f"Reference of type '{type(ref)}' is not suitable.")
+
+        shape = (cycles, self.n_base_vars + sum(self.tracked_variables.values()))
+
+        shm = SharedMemory(create=True, size=int(np.dtype(np.float64).itemsize * np.prod(shape)))
+        hist = np.ndarray(shape=shape, dtype=np.float64, buffer=shm.buf)
+        hist *= 0
+        hist[:, 0] = np.arange(0, cycles/freq, 1/freq)
 
-        # calculate number of additional columns needed
-        extra_hist_size = sum(self.tracked_variables.values())
-        # t1 - tstart, ref, pot, sensor, actuator, any additional variables
-        hist = np.zeros((maxcntr, self.n_base_vars + extra_hist_size))
-
-        # create a zero array if no ref is given
-        if ref is None:
-            ref = np.zeros(maxcntr)
+        cntr: ctypes.c_ulong = RawValue(ctypes.c_uint32)
 
-        # expand ref to array if given as integer/float (i.e. constant reference)
-        elif isinstance(ref, (int, float)):
-            ref = ref * np.ones(maxcntr)
+        process = Process(target=self._run, args=(freq, cycles, ref, cntr, shm.name, hist.shape, hist.dtype))
+        process.start()
 
         if live_plotter:
-            live_plotter.set_up(cycles, freq)
-            plot_process = live_plotter.get_process()
-            plot_process.start()
+            live_plotter.set_plot_limits_time(cycles / freq, freq)
+            live_plotter.plot(hist, cntr)
+
+        process.join()
+
+        hist = hist.copy()
+        shm.close()
+        shm.unlink()
+
+        return hist
+
+    def _run(self, freq: int | float, cycles: int, ref: Reference, cntr: ctypes.c_ulong, memname: str, shape: tuple[int, int], dtype: np.dtype):
+        shm = SharedMemory(name=memname)
+        hist = np.ndarray(shape=shape, dtype=dtype, buffer=shm.buf)
+
+        period = 1/freq
 
         with self.shield as shield:
             # need an initial write so there's something to read when we get there.
             shield.write(shield.RUN, 0)
 
             tstart = time.perf_counter()
             t0 = t1 = tstart
 
             done = False
             while not done:
                 try:
-                    print(f"\r{cntr}", end="")
-
-                    while (t1 - t0) < period:
-                        t1 = time.perf_counter()
+                    pot, sensor = shield.read()
 
                     dt = t1 - t0
                     t0 = t1
+                    ti = t1 - tstart
 
-                    pot, sensor = shield.read()
-                    raw_actuator = self.controller(t1 - tstart, dt, ref[cntr], pot, sensor)
+                    ref_i = ref(cntr.value, ti, pot)
+
+                    raw_actuator = self.controller(ti, dt, ref_i, pot, sensor)
                     actuator = shield.write(shield.RUN, raw_actuator)
 
-                    self._update_hist(hist, cntr, t1 - tstart, ref[cntr], pot, sensor, actuator)
+                    self._update_hist(hist, cntr, ti, ref_i, pot, sensor, actuator)
 
-                    if live_plotter:
-                        live_plotter.add_data_to_queue(t1 - tstart, ref[cntr], pot, sensor, actuator/(2**shield.actuator_bits/100))
+                    print(f"\r{cntr.value}", end="")
 
-                    cntr += 1
-                    if cntr == maxcntr:
+                    cntr.value += 1
+                    if cntr.value == cycles:
                         done = True
 
+                    while (t1 - t0) < period:
+                        t1 = time.perf_counter()
+
                 except KeyboardInterrupt:
                     done = True
 
             print()
+            shm.close()
 
-        # signals to terminate live plot
-        if live_plotter:
-            live_plotter.add_data_to_queue(-1, -1, -1, -1, -1)
-            plot_process.join()
-
-        return hist
-
-    def _update_hist(self, hist: npt.NDArray[np.float_], cntr: int, t: float, ref: float, pot:float, sensor: float, actuator: float):
-        """Update hist array with variables of the current iteration (cntr). If variables were added to `extra_hist_vars`, add them to the hist as well.
-
-        :param hist: array to update.
-        :type hist: npt.NDArray[np.float\_]
-        :param cntr: Iteration counter. Provides the first index to hist.
-        :type cntr: int
-        :param t: Time.
-        :type t: float
-        :param ref: Current reference value.
-        :type ref: float
-        :param sensor: Current pendulum angle
-        :type sensor: float
-        :param actuator: Current Motor value.
-        :type actuator: float
-        """
+    def _update_hist(self, hist: npt.NDArray[np.float64], cntr: int, t: float, ref: int | float, pot:float, sensor: float, actuator: int | float):
+        """Update hist array with variables of the current iteration (cntr). If variables were added to `extra_hist_vars`, add them to the hist as well."""
         hist[cntr, 0:self.n_base_vars] = t, ref, pot, sensor, actuator
         total_vars = self.n_base_vars
 
         for name, size in self.tracked_variables.items():
             hist[cntr, total_vars:total_vars+size] = getattr(self, name)
 
             total_vars += size
```

### Comparing `python_automationshield-1.0.3/src/automationshield/shields/aeroshield.py` & `python_automationshield-1.1.0/src/automationshield/shields/aeroshield.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,20 @@
         * Actuator input should be provided in percent by default.
         * Potentiometer is provided in percent by default.
         * Sensor values are converted to degrees by default.
     """
     script = "aeroshield"
     shield_id = "AE"
 
+    class PlotInfo:
+        sensor_unit = r"$\degree$"
+        sensor_type = "Angle"
+        sensor_min = 0
+        sensor_max = 180
+
     def convert_sensor_reading(self, raw: int) -> float:
         """Convert raw angle to degrees.
 
         .. math::
             \\alpha_{deg} = \\alpha_{raw} \\cdot \\frac{360}{2^{12}}
 
         :param raw: 12-bit value of angle sensor.
```

### Comparing `python_automationshield-1.0.3/src/automationshield/shields/baseshield.py` & `python_automationshield-1.1.0/src/automationshield/shields/baseshield.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,57 +11,47 @@
 class BaseShield:
     """Base class for shield devices. Handles communication with Arduino, sensor calibration and unit conversions. The class can also install the proper firmware on an Arduino.
 
     Interface:
         * Actuator input should be provided in percent by default.
         * Potentiometer is provided in percent by default.
         * Sensor values are converted to relevant physical units in the child classes.
-
-    :param TEST: Flag to write to Arduino. This flag is used to check if the correct firmware is installed. The response from the Arduino should be the C++ software version and the id of the shield.
-    :type TEST: int
-    :param RUN: Falg to write to Arduino. This flag is used for normal running of the shield device. The actuator value is applied and the Arduino responds with the potentiometer and sensor values.
-    :type RUN: int
-    :param STOP: Flag to write to Arduino. This flag is used to stop the actuator. The Arduino will stop the actuator to ensure the shield is safely stopped.
-    :type STOP: int
-    :param TIMEOUT: Time to wait after opening the serial connection before writing to the Arduino.
-    :type TIMEOUT: int
-    :param script: name of the script directory in which the ``.ino`` file for the specific shield is located.
-    :type script: str
-    :param shield_id: ID assigned to shield. This is used to check whether the correct firmware is installed on the Arduino.
-    :type shield_id: str
-    :param actuator_bits: Number of bits used for actuator.
-    :type actuator_bits: int
-    :param potentiometer_bits: Number of bits used for potentiometer.
-    :type potentiometer_bits: int
-    :param sensor_bits: Number of bits used for sensor.
-    :type sensor_bits: int
-    :param port: Port of the Arduino.
-    :type port: str
-    :param conn: Serial connection to the Arduino.
-    :type conn: serial.Serial
-    :param zero_reference: Zero reference of the sensor for calibration.
-    :type zero_reference: float
     """
     TEST = 0
+    """Flag to write to Arduino. This flag is used to check if the correct firmware is installed. The response from the Arduino should be the C++ software version and the id of the shield."""
     RUN = 1
+    """Flag to write to Arduino. This flag is used for normal running of the shield device. The actuator value is applied and the Arduino responds with the potentiometer and sensor values."""
     STOP = 2
+    """Flag to write to Arduino. This flag is used to stop the actuator. The Arduino will stop the actuator to ensure the shield is safely stopped."""
 
     # Wait time after opening connection
     TIMEOUT = 3
+    """Time to wait after opening the serial connection before writing to the Arduino."""
 
     script = ""
+    """Name of the script directory in which the ``.ino`` file for the specific shield is located."""
     shield_id = ""
+    """ID assigned to shield. This is used to check whether the correct firmware is installed on the Arduino."""
 
     actuator_bits = 8
+    """Number of bits used for actuator."""
     potentiometer_bits = 10  # resolution of system ad converter
+    """Number of bits used for potentiometer."""
     sensor_bits = 12
+    """Number of bits used for sensor."""
 
-    def __init__(self, port:Optional[str]=None) -> None:
-        """Constructor method. Create a serial connection object (without opening the connection). Will try to find the Arduino device is no port is provided.
+    class PlotInfo:
+        """This class contains information to improve the plots generated by the plotter classes in :py:mod:`automationshield.plotting`."""
+        sensor_unit = ""
+        sensor_type = ""
+        sensor_min = 0
+        sensor_max = 10
 
+    def __init__(self, port:Optional[str]=None) -> None:
+        """
         :param port: Port on which the Arduino is connected, defaults to None.
         :type port: str
         """
         if port is None:
             port = self.find_arduino()
         self.port = port
 
@@ -273,15 +263,15 @@
         """Implements the ``with`` context manager. This method calls
 
         * :py:meth:`BaseShield.open`,
         * :py:meth:`BaseShield.check_firmware`,
         * :py:meth:`BaseShield.calibrate`.
 
         :return: Shield instance.
-        :rtype: BaseShield
+        :rtype: ~automationshield.shields.BaseShield
         """
         self.open()
         self.check_firmware()
         self.calibrate()
         return self
 
     def __exit__(self, *args):
```

### Comparing `python_automationshield-1.0.3/src/automationshield/shields/floatshield.py` & `python_automationshield-1.1.0/src/automationshield/shields/floatshield.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,20 @@
         * Sensor values are provided in millimeters from the bottom of the tube.
     """
     script = "floatshield"
     shield_id = "FL"
 
     actuator_bits = 12
 
+    class PlotInfo:
+        sensor_unit = "mm"
+        sensor_type = "Distance"
+        sensor_min = 0
+        sensor_max = 320
+
     def calibrate_sensor_reading(self, sensor: int) -> int:
         """Calibrate sensor reading. 0 is taken as the ball being at the bottome of the tube.
 
         :param sensor: Raw sensor value.
         :type sensor: int
         :return: Calibrate sensor value.
         :rtype: int
```

### Comparing `python_automationshield-1.0.3/src/automationshield/shields/magnetoshield.py` & `python_automationshield-1.1.0/src/automationshield/shields/magnetoshield.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,43 +12,39 @@
         The electromagnet attracts a permanent magnet placed below the electormagnet. The position of the permanent magnet is estimated using a Hall effect sensor.
 
     Interface:
         * Actuator input should be provided in percent by default.
         * Potentiometer is provided in percent by default.
         * Sensor values are provided in Gauss by default. This class provides an additional method :py:meth:`MagnetoShield.magnet_position`, which calculates the distance of the permanent magnet from the electromagnet.
 
-    :param emagnet_height: Height of the electromagnet above ground in mm.
-    :type emagnet_height: int
-    :param magnet_low: Top of the magnet from ground - distance from Hall element in mm when the magnet is at the bottom of the tube.
-    :type magnet _low: int
-    :param magnet_high: Top of the magnet from ground - distance from Hall element in mm when the magent is at the top of the tube.
-    :type magnet_high: int
-    :param default_p1: Default value for calculating the magnet position. See :py:meth:`MagnetoShield.magnet_position`.
-    :type default_p1: float
-    :param default_p2: Default value for calculating the magnet position. See :py:meth:`MagnetoShield.magnet_position`.
-    :type default_p2: float
-    :param p1: Calibrated constant to calculate magnet position. See :py:meth:`MagnetoShield.magnet_position`.
-    :type p1: float
-    :param p2: Calibrated constant to calculate magnet position. See :py:meth:`MagnetoShield.magnet_position`.
-    :type p2: float
-
     This class does not use the :py:attr:`BaseShield.zero_reference` attribute.
     """
     script = "magnetoshield"
     shield_id = "MG"
 
     actuator_bits = 12
     sensor_bits = 10
 
+    class PlotInfo:
+        sensor_unit = "mm"
+        sensor_type = "Distance"
+        sensor_min = 12
+        sensor_max = 17
+
     emagnet_height = 20  # height of electromagnet above ground (mm)
+    """Height of the electromagnet above ground in mm."""
     magnet_low = 3  # top of magnet from ground - distance from hall element (mm)
+    """Top of the magnet from ground - distance from Hall element in mm when the magnet is at the bottom of the tube."""
     magnet_high = 8  # top of magnet from ground - distance from hall element (mm)
+    """Top of the magnet from ground - distance from Hall element in mm when the magent is at the top of the tube."""
 
     default_p1 = 3.233100
+    """Default value for calculating the magnet position. See :py:meth:`MagnetoShield.magnet_position`."""
     default_p2 = 0.220571
+    """Default value for calculating the magnet position. See :py:meth:`MagnetoShield.magnet_position`."""
 
     def __init__(self, port: str | None = None) -> None:
         super().__init__(port)
 
         self._p1 = None
         self._p2 = None
 
@@ -77,33 +73,33 @@
         :return: Raw sensor value.
         :rtype: int
         """
         return sensor
 
     @property
     def p1(self) -> float:
-        """Return ``p1`` constant calculated during calibration. If not available, return ``MagnetoShield.default_p1``.
+        """Return :math:`p_1` constant calculated during calibration. If not available, return :py:attr:`~MagnetoShield.default_p1`.
 
-        :return: ``p1`` constant.
+        :return: :math:`p_1` constant.
         :rtype: float
         """
         if self._p1:
             return self._p1
 
         return self.default_p1
 
     @p1.setter
     def p1(self, value: float):
         self._p1 = value
 
     @property
     def p2(self) -> float:
-        """Return ``p2`` constant calculated during calibration. If not available, return ``MagnetoShield.default_p2``.
+        """Return :math`p_2` constant calculated during calibration. If not available, return :py:attr:`~MagnetoShield.default_p2`.
 
-        :return: ``p2`` constant.
+        :return: :math:`p_2` constant.
         :rtype: float
         """
         if self._p2:
             return self._p2
 
         return self.default_p2
 
@@ -117,16 +113,16 @@
             The constants :math:`p_1` and :math:`p2` are calculated as follows:
 
         .. math::
             p_2 &= \\frac{ \\log{ \\left( height_{e-magnet} - magnet_{low} \\right) } - \\log{ \\left( height_{e-magnet} - magnet_{high} \\right) } } { \\log{ s_{low} } - \\log{ s_{high} } }
 
             p_1 &= \\frac{ height_{e-magnet} - magnet_{high} } { \\left( s_{high} \\right)^{p_2} }
 
-        :math:`height_{e-magnet}` corresponds to ``MagnetShield.emagnet_height``, which is the height of the electromagnet above ground. \
-            :math:`magnet_{low}` and :math:`magnet_{high}` correspond to ``MagnetShield.magnet_low`` and ``MagnetShield.magnet_high``, which are the distances from the top of the magnet to the sensor \\
+        :math:`height_{e-magnet}` corresponds to :py:attr:`~MagnetoShield.emagnet_height`, which is the height of the electromagnet above ground. \
+            :math:`magnet_{low}` and :math:`magnet_{high}` correspond to :py:attr:`~MagnetoShield.magnet_low` and :py:attr:`~MagnetoShield.magnet_high`, which are the distances from the top of the magnet to the sensor \
             in the lowest and highest position, respectively.
 
         """
         self.write(self.RUN, 0)
         time.sleep(.5)
         self.read()
         low = 0
@@ -152,17 +148,17 @@
         self.p2 = log((self.emagnet_height - self.magnet_low) / (self.emagnet_height - self.magnet_high)) / log(low/high)
         self.p1 = (self.emagnet_height - self.magnet_high) / (high ** self.p2)
 
     def magnet_position(self, sensor: float) -> float:
         """Calculate magnet distance from electromagnet using
 
         .. math::
-            y = p1 \cdot B^{p_2}
+            y = p_1 \cdot B^{p_2}
 
-        where :math:`B` is the magnetic flux density in Gauss. :math:`p1` and :math:`p2` are constants which are calculated in ``MagnetoShield.calibrate``.
+        where :math:`B` is the magnetic flux density in Gauss. :math:`p_1` and :math:`p_2` are constants which are calculated in :py:meth:`~MagnetoShield.calibrate`.
 
         The distance can vary between approximately :math:`12 mm` and :math:`17 mm`.
 
         :param sensor: Sensor value in Gauss.
         :type sensor: float
         :return: Magnet distance from electromagnet.
         :rtype: float
```

### Comparing `python_automationshield-1.0.3/PKG-INFO` & `python_automationshield-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: python-automationshield
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Python interface to AutomationShield's Arduino shields
 Home-page: https://gitlab.com/mrtreasurer/python-automationshield
 License: MIT
 Author: Bert Van den Abbeele
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.2)
+Requires-Dist: multiprocess (>=0.70.16)
 Requires-Dist: numpy (>=1.26.3)
 Requires-Dist: pyserial (>=3.5)
 Project-URL: Documentation, https://python-automationshield.readthedocs.io
 Project-URL: Repository, https://gitlab.com/mrtreasurer/python-automationshield
 Description-Content-Type: text/markdown
 
 # python-automationshield
```

