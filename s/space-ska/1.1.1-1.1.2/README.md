# Comparing `tmp/space_ska-1.1.1.tar.gz` & `tmp/space_ska-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_ska-1.1.1.tar", max compression
+gzip compressed data, was "space_ska-1.1.2.tar", max compression
```

## Comparing `space_ska-1.1.1.tar` & `space_ska-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-03-27 14:16:49.669953 space_ska-1.1.1/LICENSE
--rw-r--r--   0        0        0      512 2024-05-27 06:48:02.520937 space_ska-1.1.1/README.md
--rw-r--r--   0        0        0      776 2024-05-27 06:49:41.627623 space_ska-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      867 2024-05-27 06:50:08.811264 space_ska-1.1.1/ska/__init__.py
--rw-r--r--   0        0        0     3388 2024-05-27 06:40:01.687440 space_ska-1.1.1/ska/cache.py
--rw-r--r--   0        0        0     6799 2024-05-27 06:40:01.687440 space_ska-1.1.1/ska/cli.py
--rw-r--r--   0        0        0     7954 2024-05-23 20:17:43.615273 space_ska-1.1.1/ska/filter.py
--rw-r--r--   0        0        0     9888 2024-05-27 06:40:01.687440 space_ska-1.1.1/ska/spectrum.py
--rw-r--r--   0        0        0     3291 2024-05-23 20:17:43.583273 space_ska-1.1.1/ska/svo.py
--rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 space_ska-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 12:15:58.059475 space_ska-1.1.2/LICENSE
+-rw-r--r--   0        0        0      512 2024-05-30 08:06:11.117783 space_ska-1.1.2/README.md
+-rw-r--r--   0        0        0      777 2024-05-30 08:20:09.287924 space_ska-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      867 2024-05-30 08:20:11.539942 space_ska-1.1.2/ska/__init__.py
+-rw-r--r--   0        0        0     3388 2024-05-30 08:06:11.129783 space_ska-1.1.2/ska/cache.py
+-rw-r--r--   0        0        0     6799 2024-05-30 08:06:11.129783 space_ska-1.1.2/ska/cli.py
+-rw-r--r--   0        0        0     7954 2024-05-30 08:15:35.181786 space_ska-1.1.2/ska/filter.py
+-rw-r--r--   0        0        0    10578 2024-05-30 08:09:46.763222 space_ska-1.1.2/ska/spectrum.py
+-rw-r--r--   0        0        0     3291 2024-05-30 08:06:11.129783 space_ska-1.1.2/ska/svo.py
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 space_ska-1.1.2/PKG-INFO
```

### Comparing `space_ska-1.1.1/LICENSE` & `space_ska-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/README.md` & `space_ska-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/pyproject.toml` & `space_ska-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "space-ska"
-version = "1.1.1"
+version = "1.1.2"
 description = "Spectral-Kit for Asteroids"
 authors = ["Benoit Carry <benoit.carry@oca.eu>", "Max Mahlke"]
 license = "MIT"
 readme = "README.md"
 packages = [{'include' = 'ska'}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 requests = "^2.31.0"
 pandas = "^2.2.1"
 click = "^8.1.7"
 rich = "^13.7.1"
 astropy = "^6.0.1"
 numpy = "^1.26.4"
 matplotlib = "^3.5"
```

### Comparing `space_ska-1.1.1/ska/__init__.py` & `space_ska-1.1.2/ska/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 from .filter import Filter  # noqa
 from .spectrum import Spectrum  # noqa
 from . import svo  # noqa
 from .cache import download_sun_and_vega, download_mahlke_taxonomy  # noqa
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 # Cache location
 PATH_CACHE = os.path.join(os.path.expanduser("~"), ".cache/ska")
 os.makedirs(PATH_CACHE, exist_ok=True)
 
 # SKA Auxiliary data
 PATH_FILTER_LIST = os.path.join(PATH_CACHE, "svo_filters.txt")
```

### Comparing `space_ska-1.1.1/ska/cache.py` & `space_ska-1.1.2/ska/cache.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/ska/cli.py` & `space_ska-1.1.2/ska/cli.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/ska/filter.py` & `space_ska-1.1.2/ska/filter.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/ska/spectrum.py` & `space_ska-1.1.2/ska/spectrum.py`

 * *Files 11% similar despite different names*

```diff
@@ -149,35 +149,46 @@
 
     # --------------------------------------------------------------------------------
     # --------------------------------------------------------------------------------
     # --------------------------------------------------------------------------------
     # Color computation
 
     # --------------------------------------------------------------------------------
-    def compute_color(self, filter1, filter2, phot_sys="Vega", vega=None):
+    def compute_color(self, id_filter_1, id_filter_2, phot_sys="Vega", vega=None):
         """Computes filter_1-filter_2 color of spectrum in the requested system.
 
         Parameters
         ==========
-        filter_1: ska.Filter
+        id_filter_1: ska.Filter
 
-        filter_2: ska.Filter
+        id_filter_2: ska.Filter
 
         phot_sys : str
             Photometric system in which to report the color (default=Vega)
 
         vega : ska.Spectrum
             The spectrum of Vega
 
         Returns
         =======
         float
             The requested color
         """
 
+        # Check input filters
+        if isinstance(id_filter_1, ska.Filter):
+            filter1 = id_filter_1
+        else:
+            filter1 = ska.Filter(id_filter_1)
+        
+        if isinstance(id_filter_2, ska.Filter):
+            filter2 = id_filter_2
+        else:
+            filter2 = ska.Filter(id_filter_2)
+
         # Compute fluxes in each filter
         flux1 = filter1.compute_flux(self)
         flux2 = filter2.compute_flux(self)
 
         # Magnitude in AB photometric system
         if phot_sys == "AB":
             # Get Pivot wavelength for both filters
@@ -234,23 +245,23 @@
         spectrum = self.copy()
         spectrum.Flux = self.Flux * interpol_spectrum
         spectrum.Reflectance = False
         return spectrum
 
     # --------------------------------------------------------------------------------
     def reflectance_to_color(
-        self, filter1, filter2, phot_sys="Vega", vega=None, sun=None
+        self, id_filter_1, id_filter_2, phot_sys="Vega", vega=None, sun=None
     ):
         """Computes filter_1-filter_2 color for a reflectance spectrum.
 
         Parameters
         ==========
-        filter_1: ska.Filter
+        id_filter_1: ska.Filter or str
 
-        filter_2: ska.Filter
+        id_filter_2: ska.Filter or str
 
         phot_sys : str
             Photometric system in which to report the color (default=Vega)
 
         vega : ska.Spectrum
             Spectrum of Vega
 
@@ -259,14 +270,25 @@
 
         Returns
         =======
         float
             The requested color
         """
 
+        # Check input filters
+        if isinstance(id_filter_1, ska.Filter):
+            filter1 = id_filter_1
+        else:
+            filter1 = ska.Filter(id_filter_1)
+        
+        if isinstance(id_filter_2, ska.Filter):
+            filter2 = id_filter_2
+        else:
+            filter2 = ska.Filter(id_filter_2)
+
         # Integration grid is built from the transmission curve
         lambda_min = np.min([filter1.wave.min(), filter2.wave.min()])
         lambda_max = np.max([filter1.wave.max(), filter2.wave.max()])
 
         # Wavelength range to integrate over
         lambda_int = np.arange(lambda_min, lambda_max, 0.0005)
```

### Comparing `space_ska-1.1.1/ska/svo.py` & `space_ska-1.1.2/ska/svo.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.1.1/PKG-INFO` & `space_ska-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: space-ska
-Version: 1.1.1
+Version: 1.1.2
 Summary: Spectral-Kit for Asteroids
 License: MIT
 Author: Benoit Carry
 Author-email: benoit.carry@oca.eu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: astropy (>=6.0.1,<7.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: furo (>=2022.9.15,<2023.0.0) ; extra == "docs"
```

