# Comparing `tmp/ansys_tools_visualization_interface-0.2.0.tar.gz` & `tmp/ansys_tools_visualization_interface-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_tools_visualization_interface-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_tools_visualization_interface-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_tools_visualization_interface-0.2.0.tar` & `ansys_tools_visualization_interface-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1091 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/LICENSE
--rw-r--r--   0        0        0     4861 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/README.rst
--rw-r--r--   0        0        0     2858 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2020 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/__init__.py
--rw-r--r--   0        0        0     1180 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/__init__.py
--rw-r--r--   0        0        0     1857 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/_base.py
--rw-r--r--   0        0        0     1320 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py
--rw-r--r--   0        0        0    19281 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py
--rw-r--r--   0        0        0    13932 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py
--rw-r--r--   0        0        0     2803 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py
--rw-r--r--   0        0        0     2555 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py
--rw-r--r--   0        0        0     5102 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py
--rw-r--r--   0        0        0     1339 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-05-27 14:32:15.932858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     2990 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py
--rw-r--r--   0        0        0     4215 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3742 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py
--rw-r--r--   0        0        0     3568 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py
--rw-r--r--   0        0        0     3326 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py
--rw-r--r--   0        0        0     2311 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py
--rw-r--r--   0        0        0     3023 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/plotter.py
--rw-r--r--   0        0        0     1182 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/__init__.py
--rw-r--r--   0        0        0     3174 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/edge_plot.py
--rw-r--r--   0        0        0     4908 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py
--rw-r--r--   0        0        0     1187 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/__init__.py
--rw-r--r--   0        0        0     2920 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/clip_plane.py
--rw-r--r--   0        0        0     1641 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/color.py
--rw-r--r--   0        0        0     3825 2024-05-27 14:32:15.936858 ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/logger.py
--rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 ansys_tools_visualization_interface-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4861 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/README.rst
+-rw-r--r--   0        0        0     2858 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2236 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/__init__.py
+-rw-r--r--   0        0        0     1180 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/__init__.py
+-rw-r--r--   0        0        0     1857 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/_base.py
+-rw-r--r--   0        0        0     1320 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py
+-rw-r--r--   0        0        0    19281 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py
+-rw-r--r--   0        0        0    13953 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py
+-rw-r--r--   0        0        0     2803 2024-05-29 10:23:27.689401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py
+-rw-r--r--   0        0        0     2555 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py
+-rw-r--r--   0        0        0     5102 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py
+-rw-r--r--   0        0        0     1339 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     2990 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py
+-rw-r--r--   0        0        0     4215 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3742 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py
+-rw-r--r--   0        0        0     3568 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py
+-rw-r--r--   0        0        0     3326 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py
+-rw-r--r--   0        0        0     2311 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py
+-rw-r--r--   0        0        0     3023 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/plotter.py
+-rw-r--r--   0        0        0     1182 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/__init__.py
+-rw-r--r--   0        0        0     3174 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/edge_plot.py
+-rw-r--r--   0        0        0     4908 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/mesh_object_plot.py
+-rw-r--r--   0        0        0     1187 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/__init__.py
+-rw-r--r--   0        0        0     2920 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/clip_plane.py
+-rw-r--r--   0        0        0     1641 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/color.py
+-rw-r--r--   0        0        0     3825 2024-05-29 10:23:27.693401 ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/logger.py
+-rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 ansys_tools_visualization_interface-0.2.1/PKG-INFO
```

### Comparing `ansys_tools_visualization_interface-0.2.0/LICENSE` & `ansys_tools_visualization_interface-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/README.rst` & `ansys_tools_visualization_interface-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/pyproject.toml` & `ansys_tools_visualization_interface-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-tools-visualization-interface"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python visualization interface for PyAnsys libraries"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "pyvista >= 0.42.0,<1",
+    "pyvista >= 0.43.0,<1",
     "beartype >= 0.17.0,<1",
     "websockets >= 12.0,<13",
     "trame >= 3.6.0,<4",
     "trame-vtk >= 2.8.7,<3",
     "trame-vuetify >= 2.4.3,<3",
 ]
```

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 """Visualization Interface Tool is a Python client library for visualizing the results of Ansys simulations."""
 import importlib.metadata as importlib_metadata
 import os
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 USE_TRAME: bool = False
-DOCUMENTATION_BUILD: bool = False
+
+DOCUMENTATION_BUILD: bool = os.environ.get("PYANSYS_VISUALIZER_DOC_MODE", "false").lower() == "true"
+"""Whether the documentation is being built or not."""
+
 TESTING_MODE: bool = os.environ.get("PYANSYS_VISUALIZER_TESTMODE", "false").lower() == "true"
+"""Whether the library is being built or not, used to avoid showing plots while testing."""
 
 from ansys.tools.visualization_interface.plotter import Plotter  # noqa: F401, E402
 from ansys.tools.visualization_interface.types.edge_plot import EdgePlot  # noqa: F401, E402
 from ansys.tools.visualization_interface.types.mesh_object_plot import (  # noqa: F401, E402
     MeshObjectPlot,
 )
 from ansys.tools.visualization_interface.utils.clip_plane import ClipPlane  # noqa: F401, E402
```

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/_base.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/_base.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/pyvista.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/pyvista_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,25 +323,25 @@
         # To avoid a PyVista warning, conditionally set the Jupyter backend as not
         # all users will be within a notebnook environment
         if self.scene.notebook and jupyter_backend is None:
             jupyter_backend = "trame"
 
         # Override Jupyter backend if building docs
         if DOCUMENTATION_BUILD:
-            jupyter_backend = "static"
+            jupyter_backend = "html"
 
         # Enabling anti-aliasing by default on scene
         self.scene.enable_anti_aliasing("ssaa")
 
         # If screenshot is requested, set off_screen to True for the plotter
         if kwargs.get("screenshot") is not None:
             self.scene.off_screen = True
 
         # If running on testing, set off_screen to True for the plotter
-        if TESTING_MODE:
+        if TESTING_MODE or DOCUMENTATION_BUILD:
             self.scene.off_screen = True
 
         self.scene.show(jupyter_backend=jupyter_backend, **kwargs)
 
     def set_add_mesh_defaults(self, plotting_options: Optional[Dict]) -> None:
         """Set the default values for the plotting options.
```

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_local.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_remote.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/trame_service.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/backends/pyvista/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/plotter.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/plotter.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/edge_plot.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/edge_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/types/mesh_object_plot.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/types/mesh_object_plot.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/__init__.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/clip_plane.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/clip_plane.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/color.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/color.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/src/ansys/tools/visualization_interface/utils/logger.py` & `ansys_tools_visualization_interface-0.2.1/src/ansys/tools/visualization_interface/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_tools_visualization_interface-0.2.0/PKG-INFO` & `ansys_tools_visualization_interface-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ansys-tools-visualization-interface
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python visualization interface for PyAnsys libraries
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyvista >= 0.42.0,<1
+Requires-Dist: pyvista >= 0.43.0,<1
 Requires-Dist: beartype >= 0.17.0,<1
 Requires-Dist: websockets >= 12.0,<13
 Requires-Dist: trame >= 3.6.0,<4
 Requires-Dist: trame-vtk >= 2.8.7,<3
 Requires-Dist: trame-vuetify >= 2.4.3,<3
 Requires-Dist: ansys-sphinx-theme==0.16.2 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
```

