# Comparing `tmp/rad4sea-0.0.1.tar.gz` & `tmp/rad4sea-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad4sea-0.0.1.tar", last modified: Tue May 14 18:48:33 2024, max compression
+gzip compressed data, was "rad4sea-0.0.2.tar", last modified: Thu May 30 04:33:54 2024, max compression
```

## Comparing `rad4sea-0.0.1.tar` & `rad4sea-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:48:33.391677 rad4sea-0.0.1/
--rw-rw-rw-   0        0        0    21072 2024-04-17 05:51:37.000000 rad4sea-0.0.1/LICENCE.md
--rw-rw-rw-   0        0        0       81 2024-05-13 10:35:58.000000 rad4sea-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1065 2024-05-14 18:48:33.389943 rad4sea-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       72 2024-04-17 05:51:37.000000 rad4sea-0.0.1/README.md
--rw-rw-rw-   0        0        0      111 2024-05-13 10:36:18.000000 rad4sea-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 18:48:33.374547 rad4sea-0.0.1/rad4sea/
--rw-rw-rw-   0        0        0    12219 2024-05-14 18:47:41.000000 rad4sea-0.0.1/rad4sea/atmos.py
--rw-rw-rw-   0        0        0    54926 2024-05-13 10:11:19.000000 rad4sea-0.0.1/rad4sea/atmos_dev.ipynb
--rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.1/rad4sea/geom.py
--rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.1/rad4sea/hydros.py
--rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.1/rad4sea/lumos
--rw-rw-rw-   0        0        0      245 2024-04-17 05:51:37.000000 rad4sea-0.0.1/rad4sea/radio.py
--rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.1/rad4sea/surf.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:48:33.388561 rad4sea-0.0.1/rad4sea.egg-info/
--rw-rw-rw-   0        0        0     1065 2024-05-14 18:48:33.000000 rad4sea-0.0.1/rad4sea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-05-14 18:48:33.000000 rad4sea-0.0.1/rad4sea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:48:33.000000 rad4sea-0.0.1/rad4sea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-14 18:48:33.000000 rad4sea-0.0.1/rad4sea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:48:33.000000 rad4sea-0.0.1/rad4sea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:48:33.392191 rad4sea-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-14 18:48:06.000000 rad4sea-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:33:54.265478 rad4sea-0.0.2/
+-rw-rw-rw-   0        0        0    21072 2024-04-17 05:51:37.000000 rad4sea-0.0.2/LICENCE.md
+-rw-rw-rw-   0        0        0       81 2024-05-13 10:35:58.000000 rad4sea-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1065 2024-05-30 04:33:54.264478 rad4sea-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       72 2024-04-17 05:51:37.000000 rad4sea-0.0.2/README.md
+-rw-rw-rw-   0        0        0      111 2024-05-13 10:36:18.000000 rad4sea-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 04:33:54.256478 rad4sea-0.0.2/rad4sea/
+-rw-rw-rw-   0        0        0    12625 2024-05-30 04:33:04.000000 rad4sea-0.0.2/rad4sea/atmos.py
+-rw-rw-rw-   0        0        0    54926 2024-05-13 10:11:19.000000 rad4sea-0.0.2/rad4sea/atmos_dev.ipynb
+-rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.2/rad4sea/geom.py
+-rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.2/rad4sea/hydros.py
+-rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.2/rad4sea/lumos
+-rw-rw-rw-   0        0        0      245 2024-04-17 05:51:37.000000 rad4sea-0.0.2/rad4sea/radio.py
+-rw-rw-rw-   0        0        0        0 2024-04-17 05:51:37.000000 rad4sea-0.0.2/rad4sea/surf.py
+drwxrwxrwx   0        0        0        0 2024-05-30 04:33:54.263478 rad4sea-0.0.2/rad4sea.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-30 04:33:54.000000 rad4sea-0.0.2/rad4sea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-30 04:33:54.000000 rad4sea-0.0.2/rad4sea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 04:33:54.000000 rad4sea-0.0.2/rad4sea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 04:33:54.000000 rad4sea-0.0.2/rad4sea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 04:33:54.000000 rad4sea-0.0.2/rad4sea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 04:33:54.265478 rad4sea-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-30 04:33:21.000000 rad4sea-0.0.2/setup.py
```

### Comparing `rad4sea-0.0.1/LICENCE.md` & `rad4sea-0.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rad4sea-0.0.1/PKG-INFO` & `rad4sea-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad4sea
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for for radiometric transforms for hyperspectral seafloor/water column mapping
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rad4sea-0.0.1/rad4sea/atmos.py` & `rad4sea-0.0.2/rad4sea/atmos.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,30 @@
     s.outputs = None
     a = copy.deepcopy(s)
     # TODO: Pass the wavelength filter
     a.wavelength = Wavelength(wv)
     a.run()
     return SixSHelpers.Wavelengths.recursive_getattr(a.outputs, "pixel_radiance")
 
+# From openhsi/atmos
 def run_wavelengths(wavelengths:np.array, s, n_threads:int = 8) -> np.array:
     """Modified version of SixSHelpers.Wavelengths.run_wavelengths that has a progress bar.
     This implementation uses threading (through Python's multiprocessing API)."""
     
-    
-    with Pool(n_threads) as p, tqdm(total=len(wavelengths)) as pbar:
-        res = [p.apply_async( _sixs_run_one_wavelength, args=(s, wavelengths[i],), 
-                callback=lambda _: pbar.update(1)) for i in range(len(wavelengths))]
-        results = [r.get() for r in res]
+    try:
+        with Pool(n_threads) as p, tqdm(total=len(wavelengths)) as pbar:
+            res = [p.apply_async( _sixs_run_one_wavelength, args=(s, wavelengths[i],), 
+                    callback=lambda _: pbar.update(1)) for i in range(len(wavelengths))]
+            results = [r.get() for r in res]
+    except IndexError:
+        print('Multiprocessing failed for Py6S, running single processing with helper func from py6s')
+        
+        wv, results = SixSHelpers.Wavelengths.run_wavelengths(s, wavelengths, output_name='pixel_radiance')
+
+                
     
     return np.array(results)
 
 
 # From ISTUTOR
 def srf(x, mu, sigma):
     """
@@ -122,15 +129,15 @@
         #Viewing and sun geometry
         s.geometry = Geometry.User()
         s.geometry.day = z_time.day
         s.geometry.month = z_time.month
         
         # Position, direction of sensor
         lat = self.lat # latitude in degrees
-        lon = self.lat # longitude in degrees
+        lon = self.lon # longitude in degrees
         
         # Stand at zero now
         zen = 0
         azi = 0
         alt = self.altitude_msl / 10**3 # km
         
         date_str = z_time_str.split()[0]
@@ -139,14 +146,18 @@
 
         #Viewing and sun geometry
         s.geometry = Geometry.User()
         s.geometry.day = z_time.day
         s.geometry.month = z_time.month
         dt_str = f"{z_time.year}-{z_time.month:02d}-{z_time.day:02d} {z_time.hour:02d}:{z_time.minute:02d}:{z_time.second:02d}"
         s.geometry.from_time_and_location(lat, lon, dt_str, zen, azi)
+        
+        print(dt_str)
+        print(date_str)
+        print(f"{lon}, {lat}, {alt}")
 
 
         #Altitude
         s.altitudes = Altitudes()
         s.altitudes.set_sensor_custom_altitude(alt) # km
         s.altitudes.set_target_sea_level()
         s.ground_reflectance = GroundReflectance.HomogeneousLambertian(1) # Ground reflectance for spectralon panel
```

### Comparing `rad4sea-0.0.1/rad4sea/atmos_dev.ipynb` & `rad4sea-0.0.2/rad4sea/atmos_dev.ipynb`

 * *Files identical despite different names*

### Comparing `rad4sea-0.0.1/rad4sea.egg-info/PKG-INFO` & `rad4sea-0.0.2/rad4sea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad4sea
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for for radiometric transforms for hyperspectral seafloor/water column mapping
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rad4sea-0.0.1/setup.py` & `rad4sea-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('C:/Users/haavasl/VsCodeProjects/rad4sea/requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name='rad4sea',
-    version='0.0.1',    
+    version='0.0.2',    
     description='A Python package for for radiometric transforms for hyperspectral seafloor/water column mapping',
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type = "text/markdown",
     url='https://github.com/havardlovas/gref4hsi',
     author='Haavard Snefjellaa Loevaas',
     author_email='havard.s.lovas@ntnu.no',
     license='EUPL-1.2',
```

