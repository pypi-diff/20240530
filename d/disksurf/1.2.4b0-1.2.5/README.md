# Comparing `tmp/disksurf-1.2.4b0.tar.gz` & `tmp/disksurf-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disksurf-1.2.4b0.tar", last modified: Wed Dec  6 18:44:50 2023, max compression
+gzip compressed data, was "disksurf-1.2.5.tar", last modified: Thu May 30 17:45:00 2024, max compression
```

## Comparing `disksurf-1.2.4b0.tar` & `disksurf-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-12-06 18:44:50.763494 disksurf-1.2.4b0/
--rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:30:47.000000 disksurf-1.2.4b0/LICENSE
--rw-r--r--   0 richardteague   (501) staff       (20)     3730 2023-12-06 18:44:50.763379 disksurf-1.2.4b0/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     3297 2023-03-27 18:30:47.000000 disksurf-1.2.4b0/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-12-06 18:44:50.762686 disksurf-1.2.4b0/disksurf/
--rw-r--r--   0 richardteague   (501) staff       (20)      103 2023-03-27 18:30:47.000000 disksurf-1.2.4b0/disksurf/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    68283 2023-07-14 17:14:10.000000 disksurf-1.2.4b0/disksurf/observation.py
--rw-r--r--   0 richardteague   (501) staff       (20)    61379 2023-12-06 18:44:25.000000 disksurf-1.2.4b0/disksurf/surface.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-12-06 18:44:50.763234 disksurf-1.2.4b0/disksurf.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)     3730 2023-12-06 18:44:50.000000 disksurf-1.2.4b0/disksurf.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      250 2023-12-06 18:44:50.000000 disksurf-1.2.4b0/disksurf.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-12-06 18:44:50.000000 disksurf-1.2.4b0/disksurf.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       57 2023-12-06 18:44:50.000000 disksurf-1.2.4b0/disksurf.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        9 2023-12-06 18:44:50.000000 disksurf-1.2.4b0/disksurf.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-12-06 18:44:50.763555 disksurf-1.2.4b0/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      843 2023-12-06 18:44:35.000000 disksurf-1.2.4b0/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-30 17:45:00.056526 disksurf-1.2.5/
+-rw-r--r--   0 richardteague   (501) staff       (20)     1068 2023-03-27 18:30:47.000000 disksurf-1.2.5/LICENSE
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2024-05-30 17:45:00.056415 disksurf-1.2.5/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     3297 2023-03-27 18:30:47.000000 disksurf-1.2.5/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-30 17:45:00.055735 disksurf-1.2.5/disksurf/
+-rw-r--r--   0 richardteague   (501) staff       (20)      103 2023-03-27 18:30:47.000000 disksurf-1.2.5/disksurf/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    68534 2024-05-30 17:44:06.000000 disksurf-1.2.5/disksurf/observation.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    61379 2024-05-07 15:36:43.000000 disksurf-1.2.5/disksurf/surface.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-30 17:45:00.056271 disksurf-1.2.5/disksurf.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)     3728 2024-05-30 17:45:00.000000 disksurf-1.2.5/disksurf.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      250 2024-05-30 17:45:00.000000 disksurf-1.2.5/disksurf.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2024-05-30 17:45:00.000000 disksurf-1.2.5/disksurf.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       57 2024-05-30 17:45:00.000000 disksurf-1.2.5/disksurf.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        9 2024-05-30 17:45:00.000000 disksurf-1.2.5/disksurf.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-05-30 17:45:00.056560 disksurf-1.2.5/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      842 2024-05-30 17:43:04.000000 disksurf-1.2.5/setup.py
```

### Comparing `disksurf-1.2.4b0/LICENSE` & `disksurf-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.4b0/PKG-INFO` & `disksurf-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.4b0
+Version: 1.2.5
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.4b0 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.5 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                              [HD163296_zeroth.png]
                        _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_D_O_I_]_[_D_O_I_]
```

### Comparing `disksurf-1.2.4b0/README.md` & `disksurf-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.4b0/disksurf/observation.py` & `disksurf-1.2.5/disksurf/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,23 @@
     Args:
         path (str): Relative path to the FITS cube.
         FOV (optional[float]): Clip the image cube down to a specific
             field-of-view spanning a range ``FOV``, where ``FOV`` is in
             [arcsec].
         velocity_range (optional[tuple]): A tuple of the minimum and maximum
             velocity in [m/s] to cut the cube down to.
+        restfreq (optional[float]): A user-specified rest-frame frequency in
+            [Hz] that will override the one found in the header.
     """
 
-    def __init__(self, path, FOV=None, velocity_range=None):
-        super().__init__(path=path, FOV=FOV, velocity_range=velocity_range)
+    def __init__(self, path, FOV=None, velocity_range=None, restfreq=None):
+        super().__init__(path=path,
+                         FOV=FOV,
+                         velocity_range=velocity_range,
+                         restfreq=restfreq)
         self.data_aligned_rotated = {}
         self.mask_keplerian = {}
 
     def get_emission_surface(self, inc, PA, vlsr, x0=0.0, y0=0.0, chans=None,
             r_min=None, r_max=None, smooth=None, nsigma=None, min_SNR=5,
             force_opposite_sides=True, force_correct_shift=False,
             detect_peaks_kwargs=None, get_keplerian_mask_kwargs=None,
@@ -1156,15 +1161,15 @@
         # Plot the channel map.
 
         velocities = self.velax.copy()[chans[0]:chans[1]+1]
         nrows = np.ceil(velocities.size / 5).astype(int)
         fig, axs = plt.subplots(ncols=5, nrows=nrows, figsize=(11, 2*nrows+1),
                                 constrained_layout=True)
         for a, ax in enumerate(axs.flatten()):
-            if a >= self.velax.size:
+            if a >= velocities.size:
                 continue
             ax.imshow(self.data[chans[0]+a], origin='lower',
                       extent=self.extent, vmax=0.75*np.nanmax(self.data),
                       vmin=0.0, cmap='binary_r')
             if mask is not None:
                 ax.contour(self.xaxis, self.yaxis, mask[chans[0]+a], [0.5],
                            colors='orangered', linestyles='--', linewidths=0.5)
```

### Comparing `disksurf-1.2.4b0/disksurf/surface.py` & `disksurf-1.2.5/disksurf/surface.py`

 * *Files identical despite different names*

### Comparing `disksurf-1.2.4b0/disksurf.egg-info/PKG-INFO` & `disksurf-1.2.5/disksurf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disksurf
-Version: 1.2.4b0
+Version: 1.2.5
 Summary: Infer and reproject a disk's 3D structure.
 Home-page: https://github.com/richteague/disksurf
 Author: Richard Teague
 Author-email: rteague@mit.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: disksurf Version: 1.2.4b0 Summary: Infer and
+Metadata-Version: 2.1 Name: disksurf Version: 1.2.5 Summary: Infer and
 reproject a disk's 3D structure. Home-page: https://github.com/richteague/
 disksurf Author: Richard Teague Author-email: rteague@mit.edu License: MIT
 Classifier: Programming Language :: Python :: 3.5 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # disksurf
                              [HD163296_zeroth.png]
                        _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_D_O_I_]_[_D_O_I_]
```

### Comparing `disksurf-1.2.4b0/setup.py` & `disksurf-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="disksurf",
-    version="1.2.4b",
+    version="1.2.5",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description=("Infer and reproject a disk's 3D structure."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/richteague/disksurf",
     packages=["disksurf"],
```

