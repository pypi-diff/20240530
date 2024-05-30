# Comparing `tmp/libschrodinger-1.0.2.tar.gz` & `tmp/libschrodinger-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libschrodinger-1.0.2.tar", last modified: Thu May 30 20:06:59 2024, max compression
+gzip compressed data, was "libschrodinger-1.0.3.tar", last modified: Thu May 30 20:22:56 2024, max compression
```

## Comparing `libschrodinger-1.0.2.tar` & `libschrodinger-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.749455 libschrodinger-1.0.2/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.2/LICENSE
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:06:59.749029 libschrodinger-1.0.2/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.2/README.md
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.746284 libschrodinger-1.0.2/libschrodinger/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      236 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/__init__.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/config.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      651 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/constants.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4899 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/electron.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/figlocation.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2728 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/gauss.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4515 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/graphs.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      812 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/interaction.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1954 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/particle.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2987 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/potential.py
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      866 2024-05-30 09:54:56.000000 libschrodinger-1.0.2/libschrodinger/waveutils.py
-drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:06:59.748536 libschrodinger-1.0.2/libschrodinger.egg-info/
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/PKG-INFO
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      483 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/SOURCES.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/dependency_links.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:06:59.000000 libschrodinger-1.0.2/libschrodinger.egg-info/top_level.txt
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      633 2024-05-30 20:06:52.000000 libschrodinger-1.0.2/pyproject.toml
--rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:06:59.749555 libschrodinger-1.0.2/setup.cfg
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:22:56.035962 libschrodinger-1.0.3/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)    35149 2024-05-30 19:31:29.000000 libschrodinger-1.0.3/LICENSE
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:22:56.035642 libschrodinger-1.0.3/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      849 2024-05-30 19:45:52.000000 libschrodinger-1.0.3/README.md
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:22:56.033210 libschrodinger-1.0.3/libschrodinger/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      247 2024-05-30 20:13:20.000000 libschrodinger-1.0.3/libschrodinger/__init__.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1744 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/config.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      662 2024-05-30 20:13:30.000000 libschrodinger-1.0.3/libschrodinger/constants.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     5031 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/electron.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      699 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/figlocation.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2816 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/gauss.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     4636 2024-05-30 20:14:06.000000 libschrodinger-1.0.3/libschrodinger/graphs.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      922 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/interaction.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     2053 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/particle.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     3009 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/potential.py
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      899 2024-05-30 20:12:35.000000 libschrodinger-1.0.3/libschrodinger/waveutils.py
+drwxr-xr-x   0 bartoszg  (1000) bartoszg  (1000)        0 2024-05-30 20:22:56.035244 libschrodinger-1.0.3/libschrodinger.egg-info/
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)     1418 2024-05-30 20:22:56.000000 libschrodinger-1.0.3/libschrodinger.egg-info/PKG-INFO
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      483 2024-05-30 20:22:56.000000 libschrodinger-1.0.3/libschrodinger.egg-info/SOURCES.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)        1 2024-05-30 20:22:56.000000 libschrodinger-1.0.3/libschrodinger.egg-info/dependency_links.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       15 2024-05-30 20:22:56.000000 libschrodinger-1.0.3/libschrodinger.egg-info/top_level.txt
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)      633 2024-05-30 20:21:33.000000 libschrodinger-1.0.3/pyproject.toml
+-rw-r--r--   0 bartoszg  (1000) bartoszg  (1000)       38 2024-05-30 20:22:56.036041 libschrodinger-1.0.3/setup.cfg
```

### Comparing `libschrodinger-1.0.2/LICENSE` & `libschrodinger-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.2/PKG-INFO` & `libschrodinger-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.0.2/README.md` & `libschrodinger-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.2/libschrodinger/config.py` & `libschrodinger-1.0.3/libschrodinger/config.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.2/libschrodinger/constants.py` & `libschrodinger-1.0.3/libschrodinger/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 NS_IN_HOUR = 3_600_000_000_000
 """
 nanoseconds in an hour, needed for ETA calculations in the engine
 """
 TEST_TOLERANCE_TRESHOLD = 0.001
 """
-the tolerance threshold for lib.testutils.floateq.floateq()
+the tolerance threshold for libschrodinger.testutils.floateq.floateq()
 """
 PLT_FONT = {"fontname": "monospace"}
 """
 The fontname dict for Matplotlib
 """
```

### Comparing `libschrodinger-1.0.2/libschrodinger/electron.py` & `libschrodinger-1.0.3/libschrodinger/electron.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 import scipy
 import uuid
 
-import lib.particle
-import lib.config
-import lib.potential
-import lib.gauss
+import libschrodinger.particle
+import libschrodinger.config
+import libschrodinger.potential
+import libschrodinger.gauss
 
 
-class Electron(lib.particle.Particle):
+class Electron(libschrodinger.particle.Particle):
     """
     Basic representation of an electron in an atom.
     """
 
-    config: lib.config.Config
+    config: libschrodinger.config.Config
     """
        experiment configurations
     """
-    potential: lib.potential.Potential
+    potential: libschrodinger.potential.Potential
     """
     the potential field
             we are modeling the electron in
     """
     principal_quantum: int
     """
     principal quantum number
@@ -63,21 +63,21 @@
         self._cycle = 0
         self.T = 5
 
         self.psi = self.calculate_psi(potential)
         integ = np.sum((abs(self.psi) ** 2) * (config.dx) * (config.dy))
         self.psi /= integ ** (1 / 2)
 
-    def calculate_psi(self, potential: lib.potential.Potential):
+    def calculate_psi(self, potential: libschrodinger.potential.Potential):
         """
         Calculate the wave function for a bound electron with given n, l, m
 
         Parameters
         ----------
-        - potential: lib.potential.Potential
+        - potential: libschrodinger.potential.Potential
             - the actual potential function to model an electron in
         """
         r_norm = potential.r / (
             self.principal_quantum * self.config.a0
         )  # Normalize r for the excited state
         theta = np.arctan2(
             self.config.Y - potential.y_center, self.config.X - potential.x_center
@@ -92,25 +92,25 @@
             * r_norm
             * np.exp(-r_norm)
             * Ylm
         )
         return psi
 
     def propagate(
-        self, V: np.array, particles: list[lib.particle.Particle], frame: int
+        self, V: np.array, particles: list[libschrodinger.particle.Particle], frame: int
     ):
         """
         propagate the wave function in a potential field
 
         Parameters
         ----------
         - `V: np.array`
             - the potential field as an array
             of shape (Nx, Ny)
-        - `particles: list[lib.particle.Particle]`
+        - `particles: list[libschrodinger.particle.Particle]`
             - an array of other particles
             for inter-particle interactions
 
         """
 
         # Propagate through the Schrodinger's equation
         self.psi = self.psi * np.exp(-1j * (V) * self.config.dt / 2)
@@ -130,15 +130,15 @@
         if ((frame * self.config.dt) % self.T > 0)\
                 and ((frame * self.config.dt) % self.T < 1)\
                 and self._cycle == 0:
             if self.principal_quantum < 2:
                 # broke-ass electron, can't even afford a photon xd
                 return
             self._cycle = 1
-            p = lib.gauss.WavePacket(
+            p = libschrodinger.gauss.WavePacket(
                 self.config,
                 0.3,
                 2,
                 2,
                 self.potential.x_center,
                 self.potential.y_center,
                 0,
```

### Comparing `libschrodinger-1.0.2/libschrodinger/figlocation.py` & `libschrodinger-1.0.3/libschrodinger/figlocation.py`

 * *Files identical despite different names*

### Comparing `libschrodinger-1.0.2/libschrodinger/gauss.py` & `libschrodinger-1.0.3/libschrodinger/gauss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import uuid
 
-import lib.particle
-import lib.waveutils
-import lib.config
+import libschrodinger.particle
+import libschrodinger.waveutils
+import libschrodinger.config
 
 
-class WavePacket(lib.particle.Particle):
+class WavePacket(libschrodinger.particle.Particle):
     """
     Gaussian wave packet.
     Pretty simple representation of a photon or other alone particle
     """
 
     sigma: float
     """
@@ -36,15 +36,15 @@
     """
     X component for the velocity [EXPERIMENTAL]
     """
     vy: float
     """
     Y component for the velocity [EXPERIMENTAL]
     """
-    config: lib.config.Config
+    config: libschrodinger.config.Config
     """
     configuration for the domain
     """
     psi: np.array
     """
     the wave function  
 
@@ -70,31 +70,31 @@
             -((config.X - x0) ** 2 + (config.Y - y0) ** 2) / (2 * sigma**2)
         ) * np.exp(1j * (kx0 * config.X + ky0 * config.Y))
 
         integ = np.sum((abs(self.psi) ** 2) * (config.dx) * (config.dy))
         self.psi /= integ ** (1 / 2)
 
     def propagate(
-        self, V: np.array, particles: list[lib.particle.Particle], frame: int
+        self, V: np.array, particles: list[libschrodinger.particle.Particle], frame: int
     ):
         """
         propagate the wave function in a potential field
 
         Parameters
         ----------
         - `V: np.array`
             - the potential field as an array
             of shape (Nx, Ny)
-        - `particles: list[lib.particle.Particle]`
+        - `particles: list[libschrodinger.particle.Particle]`
             - an array of other particles
             for inter-particle interactions
 
         """
 
-        self.psi = lib.waveutils.rollwave(
+        self.psi = libschrodinger.waveutils.rollwave(
             self.config, self.psi, self.vx, self.vy)
 
         self.psi = self.psi * np.exp(-1j * (V) * self.config.dt / 2)
         self.psi = np.fft.fft2(self.psi)
         self.psi = self.psi * np.exp(
             -1j
             * (
```

### Comparing `libschrodinger-1.0.2/libschrodinger/graphs.py` & `libschrodinger-1.0.3/libschrodinger/graphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import matplotlib.pyplot as plt
 import matplotlib
 import os
 
 import numpy as np
 
-import lib.config
-import lib.figlocation
-import lib.constants
+import libschrodinger.config
+import libschrodinger.figlocation
+import libschrodinger.constants
 
 matplotlib.use("Agg")
 
 
 class GraphDisplay:
     """
     Class for displaying experiment output as a matplotlib graph into a file.
     """
 
-    config: lib.config.Config
+    config: libschrodinger.config.Config
     """
     configuration for the domain
     """
     fig: plt.figure
     """
     the actual matplotlib `matplotlib.pypylot.figure`
     """
@@ -30,15 +30,15 @@
 
     Defaults to None, in which case the graph doesn't display the frame number.
 
     Otherwise it displays the given frame number for this figure.
     """
 
     def __init__(
-        self, config: lib.config.Config, figsize=(12, 8), frameno: int | None = None
+        self, config: libschrodinger.config.Config, figsize=(12, 8), frameno: int | None = None
     ):
         self.config = config
         self.frameno = frameno
         self.fig = plt.figure(figsize=figsize)
 
     def save(self, filename: str):
         """Save the animation frame as an image file.
@@ -72,20 +72,20 @@
         """
         Draws the frame number on the graph.
 
         No need to call it, `GraphDisplay.save()` calls it automagically
             if `frameno` is not None
         """
         self.fig.text(
-            0, 0, "frame " + str(self.frameno), fontsize=10, **lib.constants.PLT_FONT
+            0, 0, "frame " + str(self.frameno), fontsize=10, **libschrodinger.constants.PLT_FONT
         )
 
     def add_figure(
         self,
-        location: lib.figlocation.FigureLocation,
+        location: libschrodinger.figlocation.FigureLocation,
         function: np.array,
         title: str = "",
         fig_type: str = "3d",
         zlim=(None, None),
         **kwargs,
     ):
         """
@@ -93,42 +93,42 @@
 
         Currently supported figure types:
         - 'color': matplotlib contourf plot with a color bar
         - '3d': 3d plot displaying the function as a surface
         - 'simple': simple 2d color plot
 
         Parameters:
-        - `location:lib.figlocation.FigureLocation`:
+        - `location:libschrodinger.figlocation.FigureLocation`:
             the location for the subplot
         - `function:np.array`: the actual function to plot
         - `title:str`: the title of the subplot
         - `fig_title:str`: the figure type
         - `cmap` and `zlim`: kwargs for matplotlib
         """
         match fig_type:
             case "color":
                 ax = self.fig.add_subplot(location.spec())
                 cs = ax.contourf(self.config.X, self.config.Y,
                                  function, **kwargs)
-                ax.set_title(title, **lib.constants.PLT_FONT)
+                ax.set_title(title, **libschrodinger.constants.PLT_FONT)
                 ax.set_xlim(0, self.config.Lx)
                 ax.set_ylim(0, self.config.Ly)
                 self.fig.colorbar(cs)
             case "3d":
                 ax = self.fig.add_subplot(location.spec(), projection="3d")
                 ax.plot_surface(self.config.X, self.config.Y,
                                 function, **kwargs)
-                ax.set_title(title, **lib.constants.PLT_FONT)
+                ax.set_title(title, **libschrodinger.constants.PLT_FONT)
                 ax.set_xlim(0, self.config.Lx)
                 ax.set_ylim(0, self.config.Ly)
                 ax.set_zlim(zlim[0], zlim[1])
             case "simple":
                 ax = self.fig.add_subplot(location.spec())
                 ax.pcolormesh(self.config.X, self.config.Y, function, **kwargs)
-                ax.set_title(title, **lib.constants.PLT_FONT)
+                ax.set_title(title, **libschrodinger.constants.PLT_FONT)
 
                 ax.set_xlim(0, self.config.Lx)
                 ax.set_ylim(0, self.config.Ly)
 
     def render_mp4(self, dirname):
         """
         renders images in `{dirname}/frame%d.png` into
```

### Comparing `libschrodinger-1.0.2/libschrodinger/particle.py` & `libschrodinger-1.0.3/libschrodinger/particle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import numpy as np
 
-import lib.config
+import libschrodinger.config
 
 
 class Particle:
     """
     Base class for all particles
     """
 
-    config: lib.config.Config
+    config: libschrodinger.config.Config
     """
     configuration for the domain
     """
     psi: np.array
     """
     the wave function
 
     a `np.array` of shape `(config.Nx, config.Ny)`
     """
     _fig_opts: dict
     """
-    Additional kwargs to `lib.graphs.GraphDisplay.add_figure`
+    Additional kwargs to `libschrodinger.graphs.GraphDisplay.add_figure`
 
     or to `matplotlib.pyplot`
     """
 
     def __init__(self, config):
         self.config = config
         self.psi = np.zeros((config.Nx, config.Ny))
         self._fig_opts = {}
 
     def propagate(
-        self, V: np.array, particles: list["lib.particle.Particle"], frame: int
+        self, V: np.array, particles: list["libschrodinger.particle.Particle"], frame: int
     ):
         """
         propagate the wave function in a potential field
 
         Parameters
         ----------
         - `V: np.array`
             - the potential field as an array
             of shape (Nx, Ny)
-        - `particles: list[lib.particle.Particle]`
+        - `particles: list[libschrodinger.particle.Particle]`
             - an array of other particles
             for inter-particle interactions
 
         """
         pass
 
-    def draw(self, graph: "lib.graphs.GraphDisplay", V: np.array, x, y, num):
+    def draw(self, graph: "libschrodinger.graphs.GraphDisplay", V: np.array, x, y, num):
         """
         Draws self as graphs (`3*num`, `3*num+1`, `3*num+2`)
         on an `x` by `y` figure in `graph`
 
         Or if this is particle number `num`
         and graphs are made on a `x` by `y` grid
         """
         graph.add_figure(
-            lib.figlocation.FigureLocation(x, y, 3 * num),
+            libschrodinger.figlocation.FigureLocation(x, y, 3 * num),
             np.angle(self.psi),
             f"Phase (particle {num})",
             "color",
         )
         graph.add_figure(
-            lib.figlocation.FigureLocation(x, y, 3 * num + 1),
+            libschrodinger.figlocation.FigureLocation(x, y, 3 * num + 1),
             np.absolute(self.psi),
             f"Absolute (particle {num})",
             "3d",
         )
 
         graph.add_figure(
-            lib.figlocation.FigureLocation(x, y, 3 * num + 2),
+            libschrodinger.figlocation.FigureLocation(x, y, 3 * num + 2),
             V,
             f"Mean potential (particle {num})",
             "3d",
             zlim=(-1, 0),
             cmap=None,
         )
```

### Comparing `libschrodinger-1.0.2/libschrodinger/potential.py` & `libschrodinger-1.0.3/libschrodinger/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 
-import lib.config
+import libschrodinger.config
 
 
 class Potential:
     """
     The base class for a potential field
     """
 
-    config: lib.config.Config
+    config: libschrodinger.config.Config
     """
     configuration for the domain
     """
     x_center: float | None
     """
     defaults to center of domain,
           the centerpoint of the potential
```

### Comparing `libschrodinger-1.0.2/libschrodinger/waveutils.py` & `libschrodinger-1.0.3/libschrodinger/waveutils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import numpy as np
 
-import lib.config
+import libschrodinger.config
 
 
-def rollwave(config: lib.config.Config, wave: np.array, vx: float, vy: float):
+def rollwave(config: libschrodinger.config.Config, wave: np.array, vx: float, vy: float):
     """
     Move a wave linearily forward by `(vx, vy)` within experiment coordinates.
     Might not work well with small distances.
 
     Parameters
     ----------
-    - `config: lib.config.Config`: the domain config
+    - `config: libschrodinger.config.Config`: the domain config
     - `wave: np.array`: the wave to move, an array of shape `(Nx, Ny)`
     - `vx: float`: the X velocity (will be normalized, taking into account dx and dt)
     - `vy: float`: the Y velocity (will be normalized, taking into account dy and dt)
 
     """
     wave = [np.roll(row, int(vy / config.dy * config.dt)) for row in wave]
     wave = np.roll(wave, int(vx / config.dx * config.dt), axis=0)
```

### Comparing `libschrodinger-1.0.2/libschrodinger.egg-info/PKG-INFO` & `libschrodinger-1.0.3/libschrodinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libschrodinger
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small package for simulating quantum-scale physics.
 Author-email: 1p22geo <1p22geodecki@gmail.com>, KacperTZSTI <kacper.m.trzop@gmail.com>
 Project-URL: Homepage, https://github.com/1p22geo/schrodinger
 Project-URL: Issues, https://github.com/1p22geo/schrodinger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `libschrodinger-1.0.2/pyproject.toml` & `libschrodinger-1.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libschrodinger"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="1p22geo", email="1p22geodecki@gmail.com" },
   { name="KacperTZSTI", email="kacper.m.trzop@gmail.com" },
 ]
 description = "A small package for simulating quantum-scale physics."
 readme = "README.md"
 requires-python = ">=3.8"
```

