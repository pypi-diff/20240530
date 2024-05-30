# Comparing `tmp/trackpy-0.6.3rc1.tar.gz` & `tmp/trackpy-unknown.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackpy-0.6.3rc1.tar", last modified: Thu May 30 20:04:48 2024, max compression
+gzip compressed data, was "dist/trackpy-unknown.tar", last modified: Mon Oct 13 17:33:12 2014, max compression
```

## Comparing `trackpy-0.6.3rc1.tar` & `trackpy-unknown.tar`

### file list

```diff
@@ -1,52 +1,29 @@
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.372724 trackpy-0.6.3rc1/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1676 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/LICENSE
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      137 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/MANIFEST.in
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1778 2024-05-30 20:04:48.372499 trackpy-0.6.3rc1/PKG-INFO
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1216 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/README.md
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     2303 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/doi.png
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      293 2024-05-30 20:04:48.373743 trackpy-0.6.3rc1/setup.cfg
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1156 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/setup.py
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.374041 trackpy-0.6.3rc1/trackpy/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      272 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/__init__.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      474 2024-05-30 20:04:48.374086 trackpy-0.6.3rc1/trackpy/_version.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1439 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/api.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    21678 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/artificial.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1482 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/diag.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    26302 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/feature.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     2425 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/filtering.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     7223 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/find.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    10029 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/framewise_data.py
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.352523 trackpy-0.6.3rc1/trackpy/linking/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      420 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/__init__.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    20837 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/find_link.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    48630 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/legacy.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    22974 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/linking.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     7518 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/partial.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    17711 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/subnet.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    19525 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/subnetlinker.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     6879 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/linking/utils.py
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.357218 trackpy-0.6.3rc1/trackpy/locate_functions/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)       54 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/locate_functions/__init__.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     6710 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/locate_functions/brightfield_ring.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     7552 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/masks.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    21030 2024-05-30 17:37:15.000000 trackpy-0.6.3rc1/trackpy/motion.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    30477 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/plots.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    19547 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/predict.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    12190 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/preprocessing.py
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.371135 trackpy-0.6.3rc1/trackpy/refine/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)      151 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/refine/__init__.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    13248 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/refine/brightfield_ring.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    26177 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/refine/center_of_mass.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    58857 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/refine/least_squares.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    18284 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/static.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)       40 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/tracking.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     3078 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/try_numba.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     4513 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/uncertainty.py
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    12833 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/trackpy/utils.py
-drwxr-xr-x   0 nxk913   (960861014) PSU\Domain Users (357253257)        0 2024-05-30 20:04:48.371677 trackpy-0.6.3rc1/trackpy.egg-info/
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1778 2024-05-30 20:04:47.000000 trackpy-0.6.3rc1/trackpy.egg-info/PKG-INFO
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)     1023 2024-05-30 20:04:48.000000 trackpy-0.6.3rc1/trackpy.egg-info/SOURCES.txt
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)        1 2024-05-30 20:04:47.000000 trackpy-0.6.3rc1/trackpy.egg-info/dependency_links.txt
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)       86 2024-05-30 20:04:47.000000 trackpy-0.6.3rc1/trackpy.egg-info/requires.txt
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)        8 2024-05-30 20:04:47.000000 trackpy-0.6.3rc1/trackpy.egg-info/top_level.txt
--rw-r--r--   0 nxk913   (960861014) PSU\Domain Users (357253257)    62436 2024-05-10 15:43:27.000000 trackpy-0.6.3rc1/versioneer.py
+drwxr-xr-x   0 danielallan   (501) staff       (20)        0 2014-10-13 17:33:12.000000 trackpy-unknown/
+-rw-r--r--   0 danielallan   (501) staff       (20)     2303 2014-08-13 13:54:23.000000 trackpy-unknown/doi.png
+-rw-r--r--   0 danielallan   (501) staff       (20)    10482 2014-08-13 12:44:48.000000 trackpy-unknown/ez_setup.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     1676 2014-08-13 12:44:48.000000 trackpy-unknown/LICENSE
+-rw-r--r--   0 danielallan   (501) staff       (20)      157 2014-10-13 17:31:58.000000 trackpy-unknown/MANIFEST.in
+-rw-r--r--   0 danielallan   (501) staff       (20)    12717 2014-10-13 17:33:12.000000 trackpy-unknown/PKG-INFO
+-rw-r--r--   0 danielallan   (501) staff       (20)    10518 2014-09-11 19:21:10.000000 trackpy-unknown/README.md
+-rw-r--r--   0 danielallan   (501) staff       (20)       40 2014-10-03 18:17:35.000000 trackpy-unknown/setup.cfg
+-rw-r--r--   0 danielallan   (501) staff       (20)     1659 2014-10-03 18:17:35.000000 trackpy-unknown/setup.py
+drwxr-xr-x   0 danielallan   (501) staff       (20)        0 2014-10-13 17:33:12.000000 trackpy-unknown/trackpy/
+-rw-r--r--   0 danielallan   (501) staff       (20)      236 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/__init__.py
+-rw-r--r--   0 danielallan   (501) staff       (20)      386 2014-10-13 17:33:12.000000 trackpy-unknown/trackpy/_version.py
+-rw-r--r--   0 danielallan   (501) staff       (20)      470 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/api.py
+-rw-r--r--   0 danielallan   (501) staff       (20)      756 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/diag.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    29756 2014-10-06 17:06:16.000000 trackpy-unknown/trackpy/feature.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     2472 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/filtering.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     9701 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/framewise_data.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    48086 2014-10-06 17:06:16.000000 trackpy-unknown/trackpy/linking.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     1120 2014-10-06 17:06:16.000000 trackpy-unknown/trackpy/masks.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    15601 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/motion.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    15269 2014-10-06 17:06:16.000000 trackpy-unknown/trackpy/plots.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    14274 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/predict.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     2370 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/preprocessing.py
+-rw-r--r--   0 danielallan   (501) staff       (20)       40 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/tracking.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     4168 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/try_numba.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     2299 2014-09-11 19:21:10.000000 trackpy-unknown/trackpy/uncertainty.py
+-rw-r--r--   0 danielallan   (501) staff       (20)     5660 2014-10-03 18:06:26.000000 trackpy-unknown/trackpy/utils.py
+-rw-r--r--   0 danielallan   (501) staff       (20)       46 2014-08-03 21:01:18.000000 trackpy-unknown/trackpy/version.py
+-rw-r--r--   0 danielallan   (501) staff       (20)    35319 2014-09-11 19:21:10.000000 trackpy-unknown/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `trackpy-0.6.3rc1/LICENSE` & `trackpy-unknown/LICENSE`

 * *Files identical despite different names*

### Comparing `trackpy-0.6.3rc1/doi.png` & `trackpy-unknown/doi.png`

 * *Files identical despite different names*

### Comparing `trackpy-0.6.3rc1/setup.py` & `trackpy-unknown/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,39 @@
-import os
-import versioneer
-from setuptools import setup
+# This downloads and install setuptools if it is not installed.
+from ez_setup import use_setuptools
+use_setuptools()
 
+import os
+import sys
+import warnings
 
+# try bootstrapping setuptools if it doesn't exist
 try:
-    descr = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
-except OSError:
-    descr = ''
+    import pkg_resources
+    try:
+        pkg_resources.require("setuptools>=0.6c5")
+    except pkg_resources.VersionConflict:
+        from ez_setup import use_setuptools
+        use_setuptools(version="0.6c5")
+    from setuptools import setup, Extension
+    _have_setuptools = True
+except ImportError:
+    # no setuptools installed
+    from numpy.distutils.core import setup
+    _have_setuptools = False
+
+import versioneer
+versioneer.VCS = 'git'
+versioneer.versionfile_source = 'trackpy/_version.py'
+versioneer.versionfile_build = 'trackpy/_version.py'
+versioneer.tag_prefix = 'v'
+versioneer.parentdir_prefix = '.'
+
+def read(fname):
+    return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 # In some cases, the numpy include path is not present by default.
 # Let's try to obtain it.
 try:
     import numpy
 except ImportError:
     ext_include_dirs = []
@@ -21,19 +44,14 @@
     name = "trackpy",
     version = versioneer.get_version(),
     cmdclass = versioneer.get_cmdclass(),
     description = "particle-tracking toolkit",
     author = "Trackpy Contributors",
     author_email = "daniel.b.allan@gmail.com",
     url = "https://github.com/soft-matter/trackpy",
-    install_requires = ['numpy>=1.18', 'scipy>=1.4', 'pandas>=1', 'pyyaml', 'matplotlib', "looseversion>=1.0.1"],
-    extras_require={"test": "pytest"},
-    python_requires=">=3.8",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-    ],
-    packages = ['trackpy', 'trackpy.refine', 'trackpy.linking', 'trackpy.locate_functions'],
-    long_description = descr,
-    long_description_content_type='text/markdown'
+    install_requires = ['numpy', 'scipy', 'six', 'pandas',
+                        'pyyaml', 'matplotlib', 'pims'],
+    packages = ['trackpy'],
+    long_description = read('README.md'),
 )
 
 setup(**setup_parameters)
```

### Comparing `trackpy-0.6.3rc1/trackpy/feature.py` & `trackpy-unknown/trackpy/feature.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,643 +1,728 @@
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
 import warnings
-import logging
-from functools import partial
 
 import numpy as np
 import pandas as pd
-
-from .preprocessing import (bandpass, convert_to_int, invert_image,
-                            scalefactor_to_gamut)
-from .utils import (record_meta, validate_tuple, is_isotropic,
-                    default_pos_columns, default_size_columns,
-                    pandas_concat, get_pool)
-from .find import grey_dilation, where_close
-from .refine import refine_com, refine_com_arr
-from .masks import (binary_mask, N_binary_mask, r_squared_mask,
-                    x_squared_masks, cosmask, sinmask)
-from .uncertainty import _static_error, measure_noise
+from scipy import ndimage
+from scipy import stats
+from scipy.spatial import cKDTree
+from pandas import DataFrame, Series
+
+from . import uncertainty
+from .preprocessing import bandpass, scale_to_gamut
+from .utils import record_meta, print_update
+from .masks import *
 import trackpy  # to get trackpy.__version__
 
-logger = logging.getLogger(__name__)
-
-
-def minmass_v03_change(raw_image, old_minmass, preprocess=True,
-                       invert=False, noise_size=1, smoothing_size=None,
-                       threshold=None):
-    """Convert minmass value from v0.2.4 to v0.3.
+from .try_numba import try_numba_autojit, NUMBA_AVAILABLE
 
-    From trackpy version 0.3.0, the mass calculation is changed. Before
-    version 0.3.0 the mass was calculated from a rescaled image. From version
-    0.3.0, this rescaling is compensated at the end so that the mass reflects
-    the actual intensities in the image.
-
-    This function calculates the scalefactor between the old and new mass
-    and applies it to calculate the new minmass filter value.
-
-    Parameters
-    ----------
-    raw_image : ndarray
-    old_minmass : number
-    preprocess : boolean, optional
-        Defaults to True
-    invert : boolean, optional
-        Defaults to False
-    noise_size : number, optional
-        Defaults to 1
-    smoothing_size : number, optional
-        Required when preprocessing. In locate, it equals diameter by default.
-    threshold : number, optional
-
-    Returns
-    -------
-    New minmass
-    """
-    if preprocess and smoothing_size is None:
-        raise ValueError('Please specify the smoothing size. By default, this '
-                         'equals diameter.')
-
-    if np.issubdtype(raw_image.dtype, np.integer):
-        dtype = raw_image.dtype
-        if invert:
-            raw_image = raw_image ^ np.iinfo(dtype).max
-    else:
-        dtype = np.uint8
-        if invert:
-            raw_image = 1 - raw_image
-
-    if preprocess:
-        image = bandpass(raw_image, noise_size, smoothing_size, threshold)
-    else:
-        image = raw_image
 
-    scale_factor = scalefactor_to_gamut(image, dtype)
+def local_maxima(image, radius, separation, percentile=64):
+    """Find local maxima whose brightness is above a given percentile."""
 
-    return old_minmass / scale_factor
+    ndim = image.ndim
+    # Compute a threshold based on percentile.
+    not_black = image[np.nonzero(image)]
+    if len(not_black) == 0:
+        warnings.warn("Image is completely black.", UserWarning)
+        return np.empty((0, ndim))
+    threshold = stats.scoreatpercentile(not_black, percentile)
+
+    # The intersection of the image with its dilation gives local maxima.
+    if not np.issubdtype(image.dtype, np.integer):
+        raise TypeError("Perform dilation on exact (i.e., integer) data.")
+    footprint = binary_mask(radius, ndim, separation)
+    dilation = ndimage.grey_dilation(image, footprint=footprint,
+                                     mode='constant')
+    maxima = np.vstack(np.where((image == dilation) & (image > threshold))).T
+    if not np.size(maxima) > 0:
+        warnings.warn("Image contains no local maxima.", UserWarning)
+        return np.empty((0, ndim))
 
+    # Flat peaks return multiple nearby maxima. Eliminate duplicates.
+    while True:
+        duplicates = cKDTree(maxima, 30).query_pairs(separation)
+        if len(duplicates) == 0:
+            break
+        to_drop = []
+        for pair in duplicates:
+            # Take the average position.
+            # This is just a starting point, so we won't go into subpx precision here.
+            merged = maxima[pair[0]]
+            merged = maxima[[pair[0], pair[1]]].mean(0).astype(int)
+            maxima[pair[0]] = merged  # overwrite one
+            to_drop.append(pair[1])  # queue other to be dropped
+        maxima = np.delete(maxima, to_drop, 0)
+
+    # Do not accept peaks near the edges.
+    shape = np.array(image.shape)
+    margin = int(separation) // 2
+    near_edge = np.any((maxima < margin) | (maxima > (shape - margin)), 1)
+    maxima = maxima[~near_edge]
+    if not np.size(maxima) > 0:
+        warnings.warn("All local maxima were in the margins.", UserWarning)
+
+    # Return coords in as a numpy array shaped so it can be passed directly
+    # to the DataFrame constructor.
+    return maxima 
 
-def minmass_v04_change(raw_image, old_minmass, diameter, preprocess=True,
-                       old_smoothing_size=None, new_smoothing_size=None):
-    """Convert minmass value from v0.3 to v0.4.
-
-    From trackpy version 0.4.0, the default image preprocessing is changed.
-    Before version 0.4.0 a blurred out image (rolling or boxcar average) with
-    a circular kernel with radius `diameter` was subtracted from the image
-    before refinement and mass calculation. From version 0.4.0, this has
-    changed to a square kernel with sides `diameter`, more or less twice as
-    small. This increases tracking accuracy, and reduces the mass.
-
-    This function estimates this difference and applies it to calculate the
-    new minmass value.
 
-    Here the following approximate relation between the "real" mass of the
-    feature and the mass apparent from the bandpassed image is used:
+def estimate_mass(image, radius, coord):
+    "Compute the total brightness in the neighborhood of a local maximum."
+    square = [slice(c - radius, c + radius + 1) for c in coord]
+    neighborhood = binary_mask(radius, image.ndim)*image[square]
+    return np.sum(neighborhood)
 
-    .. math::
 
-        M_{bp} = M_{real} \\left( 1 - \\frac{n_r}{n_{bp}} \\right)
+def estimate_size(image, radius, coord, estimated_mass):
+    "Compute the total brightness in the neighborhood of a local maximum."
+    square = [slice(c - radius, c + radius + 1) for c in coord]
+    neighborhood = binary_mask(radius, image.ndim)*image[square]
+    Rg = np.sqrt(np.sum(r_squared_mask(radius, image.ndim)*neighborhood)/
+                 estimated_mass)
+    return Rg
 
-    Where :math:`n_r` denotes the number of pixels in the (circular)
-    refine mask and :math:`n_{bp}` the number of pixels in the (square)
-    rolling average kernel.
+# center_of_mass can have divide-by-zero errors, avoided thus:
+def _safe_center_of_mass(x, radius):
+    result = np.array(ndimage.center_of_mass(x))
+    if np.isnan(result).any():
+        return np.zeros_like(result) + radius
+    else:
+        return result
 
-    This follows from a simple model where the bandpassed image :math:`I_{bp}`
-    relates to the "real" feature :math:`F` and the noise :math:`N` by:
 
-    .. math::
+def refine(raw_image, image, radius, coords, max_iterations=10, engine='auto',
+           characterize=True, walkthrough=False):
+    """Find the center of mass of a bright feature starting from an estimate.
 
-        I_{bp} = F + N - \\left(N + \\frac{M_{real}}{n_{bp}} \\right)
+    Characterize the neighborhood of a local maximum, and iteratively
+    hone in on its center-of-brightness. Return its coordinates, integrated
+    brightness, size (Rg), eccentricity (0=circular), and signal strength.
 
     Parameters
     ----------
-    raw_image : ndarray
-    old_minmass : number
-    diameter : number or tuple
-        Odd-valued number that is used in locate
-    preprocess : boolean, optional
-        Defaults to True. Minmass is not changed when preprocess=False.
-    old_smoothing_size : number or tuple, optional
-        The smoothing size used in the old (pre v0.4) trackpy version (the
-        radius of the circular kernel). Defaults to diameter.
-    new_smoothing_size : number or tuple, optional
-        The smoothing size used in the new (post v0.4) trackpy version (the
-        size of the sides of the square kernel). Defaults to diameter.
-
-    Returns
-    -------
-    New minmass
+    raw_image : array (any dimensions)
+        used for final characterization
+    image : array (any dimension)
+        processed image, used for locating center of mass
+    coord : array
+        estimated position
+    max_iterations : integer
+        max number of loops to refine the center of mass, default 10
+    characterize : boolean, True by default
+        Compute and return mass, size, eccentricity, signal.
+    walkthrough : boolean, False by default
+        Print the offset on each loop and display final neighborhood image.
+    engine : {'python', 'numba'}
+        Numba is faster if available, but it cannot do walkthrough.
     """
-    if not preprocess:
-        return old_minmass
-
-    ndim = raw_image.ndim
-    diameter = validate_tuple(diameter, ndim)
-    if old_smoothing_size is None:
-        old_smoothing_size = diameter
-    else:
-        old_smoothing_size = validate_tuple(old_smoothing_size, ndim)
-    if new_smoothing_size is None:
-        new_smoothing_size = diameter
+    # Main loop will be performed in separate function.
+    if engine == 'auto':
+        if NUMBA_AVAILABLE:
+            engine = 'numba'
+        else:
+            engine = 'python'
+    if engine == 'python':
+        coords = np.array(coords)  # a copy, will not modify in place
+        results = _refine(raw_image, image, radius, coords, max_iterations,
+                          characterize, walkthrough)
+    elif engine == 'numba':
+        if not NUMBA_AVAILABLE:
+            warnings.warn("numba could not be imported. Without it, the "
+                          "'numba' engine runs very slow. Use the 'python' "
+                          "engine or install numba.", UserWarning)
+        if image.ndim != 2:
+            raise NotImplementedError("The numba engine only supports 2D "
+                                      "images. You can extend it if you feel "
+                                      "like a hero.")
+        if walkthrough:
+            raise ValueError("walkthrough is not availabe in the nubma engine")
+        # Do some extra prep in pure Python that can't be done in numba.
+        coords = np.array(coords, dtype=np.float_)
+        shape = np.array(image.shape, dtype=np.int16)  # array, not tuple
+        mask = binary_mask(radius, image.ndim)
+        r2_mask = r_squared_mask(radius, image.ndim)
+        cmask = cosmask(radius)
+        smask = sinmask(radius)
+        results = _numba_refine(raw_image, image, int(radius), coords,
+                                int(max_iterations), characterize,
+                                shape, mask, r2_mask, cmask, smask)
     else:
-        new_smoothing_size = validate_tuple(new_smoothing_size, ndim)
-
-    radius = tuple(int(d / 2) for d in diameter)
-    old_bp_size = tuple(s * 2 + 1 for s in old_smoothing_size)
+        raise ValueError("Available engines are 'python' and 'numba'")
+    return results
 
-    n_px_refine = N_binary_mask(radius, ndim)
-    n_px_old_bp = N_binary_mask(old_bp_size, ndim)
-    n_px_new_bp = np.prod(new_smoothing_size)
 
-    real_minmass = old_minmass / (1 - n_px_refine / n_px_old_bp)
-    new_minmass = real_minmass * (1 - n_px_refine / n_px_new_bp)
-    return new_minmass
-
-
-def local_maxima(image, radius, percentile=64, margin=None):
-    """Find local maxima whose brightness is above a given percentile.
-    This function will be deprecated. Please use the routines in trackpy.find,
-    with the minimum separation between features as second argument.
-
-    Parameters
-    ----------
-    image : ndarray
-        For best performance, provide an integer-type array. If the type is not
-        of integer-type, the image will be normalized and coerced to uint8.
-    radius : the radius of the circular grey dilation kernel, which is the
-        minimum separation between maxima
-    percentile : chooses minimum grayscale value for a local maximum
-    margin : zone of exclusion at edges of image. Defaults to radius.
-            A smarter value is set by locate().
-    """
-    warnings.warn("Local_maxima will be deprecated: please use routines in "
-                  "trackpy.find", PendingDeprecationWarning)
-    return grey_dilation(image, radius, percentile, margin)
+# (This is pure Python. A numba variant follows below.)
+def _refine(raw_image, image, radius, coords, max_iterations,
+            characterize, walkthrough):
+    SHIFT_THRESH = 0.6
+    GOOD_ENOUGH_THRESH = 0.005
+
+    ndim = image.ndim
+    mask = binary_mask(radius, ndim)
+    slices = [[slice(c - radius, c + radius + 1) for c in coord]
+              for coord in coords]
+
+    # Declare arrays that we will fill iteratively through loop.
+    N = coords.shape[0]
+    final_coords = np.empty_like(coords, dtype=np.float64)
+    mass = np.empty(N, dtype=np.float64)
+    Rg = np.empty(N, dtype=np.float64)
+    ecc = np.empty(N, dtype=np.float64)
+    signal = np.empty(N, dtype=np.float64)
+
+    for feat in range(N):
+        coord = coords[feat]
+
+        # Define the circular neighborhood of (x, y).
+        square = slices[feat]
+        neighborhood = mask*image[square]
+        cm_n = _safe_center_of_mass(neighborhood, radius)
+        cm_i = cm_n - radius + coord  # image coords
+        allow_moves = True
+        for iteration in range(max_iterations):
+            off_center = cm_n - radius
+            if walkthrough:
+                print_update(off_center)
+            if np.all(np.abs(off_center) < GOOD_ENOUGH_THRESH):
+                break  # Accurate enough.
+
+            # If we're off by more than half a pixel in any direction, move.
+            elif np.any(np.abs(off_center) > SHIFT_THRESH) & allow_moves:
+                # In here, coord is an integer.
+                new_coord = coord
+                new_coord[off_center > SHIFT_THRESH] += 1
+                new_coord[off_center < -SHIFT_THRESH] -= 1
+                # Don't move outside the image!
+                upper_bound = np.array(image.shape) - 1 - radius
+                new_coord = np.clip(new_coord, radius, upper_bound).astype(int)
+                # Update slice to shifted position.
+                square = [slice(c - radius, c + radius + 1) for c in new_coord]
+                neighborhood = mask*image[square]
 
+            # If we're off by less than half a pixel, interpolate.
+            else:
+                # Here, coord is a float. We are off the grid.
+                neighborhood = ndimage.shift(neighborhood, -off_center,
+                                             order=2, mode='constant', cval=0)
+                new_coord = coord + off_center
+                # Disallow any whole-pixels moves on future iterations.
+                allow_moves = False
+
+            cm_n = _safe_center_of_mass(neighborhood, radius)  # neighborhood
+            cm_i = cm_n - radius + new_coord  # image coords
+            coord = new_coord
+        # matplotlib and ndimage have opposite conventions for xy <-> yx.
+        final_coords[feat] = cm_i[..., ::-1]
+
+        if walkthrough:
+            import matplotlib.pyplot as plt
+            plt.imshow(neighborhood)
+
+        # Characterize the neighborhood of our final centroid.
+        mass[feat] = neighborhood.sum()
+        if not characterize:
+            continue  # short-circuit loop
+        Rg[feat] = np.sqrt(np.sum(r_squared_mask(radius, ndim)*
+                                  neighborhood)/mass[feat])
+        # I only know how to measure eccentricity in 2D.
+        if ndim == 2:
+            ecc[feat] = np.sqrt(np.sum(neighborhood*cosmask(radius))**2 +
+                          np.sum(neighborhood*sinmask(radius))**2)
+            ecc[feat] /= (mass[feat] - neighborhood[radius, radius] + 1e-6)
+        else:
+            ecc[feat] = np.nan
+        raw_neighborhood = mask*raw_image[square]
+        signal[feat] = raw_neighborhood.max()  # black_level subtracted later
 
-def estimate_mass(image, radius, coord):
-    "Compute the total brightness in the neighborhood of a local maximum."
-    square = [slice(c - rad, c + rad + 1) for c, rad in zip(coord, radius)]
-    neighborhood = binary_mask(radius, image.ndim)*image[square]
-    return np.sum(neighborhood)
+    if not characterize:
+        result = np.column_stack([final_coords, mass])
+    else:
+        result = np.column_stack([final_coords, mass, Rg, ecc, signal])
+    return result
 
+def _get_numba_refine_locals():
+    """Establish types of local variables in _numba_refine(), in a way that's safe if there's no numba."""
+    try:
+        from numba import double, int_
+    except ImportError:
+        return {}
+    else:
+        return dict(square0=int_, square1=int_, square_size=int_, Rg_=double, ecc_=double)
 
-def estimate_size(image, radius, coord, estimated_mass):
-    "Compute the total brightness in the neighborhood of a local maximum."
-    square = [slice(c - rad, c + rad + 1) for c, rad in zip(coord, radius)]
-    neighborhood = binary_mask(radius, image.ndim)*image[square]
-    Rg = np.sqrt(np.sum(r_squared_mask(radius, image.ndim) * neighborhood) /
-                 estimated_mass)
-    return Rg
+@try_numba_autojit(locals=_get_numba_refine_locals())
+def _numba_refine(raw_image, image, radius, coords, max_iterations,
+                  characterize, shape, mask, r2_mask, cmask, smask):
+    SHIFT_THRESH = 0.6
+    GOOD_ENOUGH_THRESH = 0.01
+
+    square_size = 2*radius + 1
+
+    # Declare arrays that we will fill iteratively through loop.
+    N = coords.shape[0]
+    final_coords = np.empty_like(coords, dtype=np.float_)
+    mass = np.empty(N, dtype=np.float_)
+    Rg = np.empty(N, dtype=np.float_)
+    ecc = np.empty(N, dtype=np.float_)
+    signal = np.empty(N, dtype=np.float_)
+    coord = np.empty((2,), dtype=np.float_)
+
+    # Buffer arrays
+    cm_n = np.empty(2, dtype=np.float_)
+    cm_i = np.empty(2, dtype=np.float_)
+    off_center = np.empty(2, dtype=np.float_)
+    new_coord = np.empty((2,), dtype=np.int_)
+
+    for feat in range(N):
+        # Define the circular neighborhood of (x, y).
+        for dim in range(2):
+            coord[dim] = coords[feat, dim]
+            cm_n[dim] = 0.
+        square0 = coord[0] - radius
+        square1 = coord[1] - radius
+        mass_ = 0.0
+        for i in range(square_size):
+            for j in range(square_size):
+                if mask[i, j] != 0:
+                    px = image[square0 + i, square1 + j]
+                    cm_n[0] += px*i
+                    cm_n[1] += px*j
+                    mass_ += px
+
+        for dim in range(2):
+            cm_n[dim] /= mass_
+            cm_i[dim] = cm_n[dim] - radius + coord[dim]
+        allow_moves = True
+        for iteration in range(max_iterations):
+            for dim in range(2):
+                off_center[dim] = cm_n[dim] - radius
+            for dim in range(2):
+                if abs(off_center[dim]) > GOOD_ENOUGH_THRESH:
+                    break  # Proceed through iteration.
+            else:
+                break
 
+            # If we're off by more than half a pixel in any direction, move.
+            do_move = False
+            if allow_moves:
+                for dim in range(2):
+                    if abs(off_center[dim]) > SHIFT_THRESH:
+                        do_move = True
+                        break
+
+            if do_move:
+                # In here, coord is an integer.
+                for dim in range(2):
+                    new_coord[dim] = int(round(coord[dim]))
+                    oc = off_center[dim]
+                    if oc > SHIFT_THRESH:
+                        new_coord[dim] += 1
+                    elif oc < - SHIFT_THRESH:
+                        new_coord[dim] += -1
+                    # Don't move outside the image!
+                    if new_coord[dim] < radius:
+                        new_coord[dim] = radius
+                    upper_bound = shape[dim] - radius - 1
+                    if new_coord[dim] > upper_bound:
+                        new_coord[dim] = upper_bound
+                # Update slice to shifted position.
+                square0 = new_coord[0] - radius
+                square1 = new_coord[1] - radius
+                for dim in range(2):
+                     cm_n[dim] = 0.
 
-def refine(*args, **kwargs):
-    """
-    Deprecated.
+            # If we're off by less than half a pixel, interpolate.
+            else:
+                break
+                # TODO Implement this for numba.
+                # Remember to zero cm_n somewhere in here.
+                # Here, coord is a float. We are off the grid.
+                # neighborhood = ndimage.shift(neighborhood, -off_center,
+                #                              order=2, mode='constant', cval=0)
+                # new_coord = np.float_(coord) + off_center
+                # Disallow any whole-pixels moves on future iterations.
+                # allow_moves = False
+
+            # cm_n was re-zeroed above in an unrelated loop
+            mass_ = 0.
+            for i in range(square_size):
+                for j in range(square_size):
+                    if mask[i, j] != 0:
+                        px = image[square0 + i, square1 + j]
+                        cm_n[0] += px*i
+                        cm_n[1] += px*j
+                        mass_ += px
+
+            for dim in range(2):
+                cm_n[dim] /= mass_
+                cm_i[dim] = cm_n[dim] - radius + new_coord[dim]
+                coord[dim] = new_coord[dim]
+        # matplotlib and ndimage have opposite conventions for xy <-> yx.
+        final_coords[feat, 0] = cm_i[1]
+        final_coords[feat, 1] = cm_i[0]
+
+        # Characterize the neighborhood of our final centroid.
+        mass_ = 0.
+        Rg_ = 0.
+        ecc1 = 0.
+        ecc2 = 0.
+        signal_ = 0.
+        for i in range(square_size):
+            for j in range(square_size):
+                if mask[i, j] != 0:
+                    px = image[square0 + i, square1 + j]
+                    mass_ += px
+                    # Will short-circuiting if characterize=False slow it down?
+                    if not characterize:
+                        continue
+                    Rg_ += r2_mask[i, j]*px
+                    ecc1 += cmask[i, j]*px
+                    ecc2 += smask[i, j]*px
+                    raw_px = raw_image[square0 + i, square1 + j]
+                    if raw_px > signal_:
+                        signal_ = px
+        Rg_ = np.sqrt(Rg_/mass_)
+        mass[feat] = mass_
+        if characterize:
+            Rg[feat] = Rg_
+            center_px = image[square0 + radius, square1 + radius]
+            ecc_ = np.sqrt(ecc1**2 + ecc2**2)/(mass_ - center_px + 1e-6)
+            ecc[feat] = ecc_
+            signal[feat] = signal_  # black_level subtracted later
 
-    See also
-    --------
-    trackpy.refine.refine_com
-    """
-    warnings.warn("trackpy.feature.refine is deprecated: please use routines in "
-                  "trackpy.refine", PendingDeprecationWarning)
-    return refine_com(*args, **kwargs)
+    if not characterize:
+        result = np.column_stack([final_coords, mass])
+    else:
+        result = np.column_stack([final_coords, mass, Rg, ecc, signal])
+    return result
 
 
-def locate(raw_image, diameter, minmass=None, maxsize=None, separation=None,
+def locate(raw_image, diameter, minmass=100., maxsize=None, separation=None,
            noise_size=1, smoothing_size=None, threshold=None, invert=False,
            percentile=64, topn=None, preprocess=True, max_iterations=10,
-           filter_before=None, filter_after=None,
+           filter_before=True, filter_after=True,
            characterize=True, engine='auto'):
-    """Locate Gaussian-like blobs of some approximate size in an image.
+    """Locate Gaussian-like blobs of a given approximate size.
 
     Preprocess the image by performing a band pass and a threshold.
     Locate all peaks of brightness, characterize the neighborhoods of the peaks
-    and take only those with given total brightness ("mass"). Finally,
+    and take only those with given total brightnesss ("mass"). Finally,
     refine the positions of each peak.
 
     Parameters
     ----------
-    raw_image : array (any dimensions)
-        Image used for final characterization. Ideally, pixel values of
-        this image are not rescaled, but it can also be identical to
-        ``image``.
-    image : array (same size as raw_image)
-        Processed image used for centroid-finding and most particle
-        measurements.
-    diameter : odd integer or tuple of odd integers
-        This may be a single number or a tuple giving the feature's
-        extent in each dimension, useful when the dimensions do not have
-        equal resolution (e.g. confocal microscopy). The tuple order is the
-        same as the image shape, conventionally (z, y, x) or (y, x). The
-        number(s) must be odd integers. When in doubt, round up.
-    minmass : float
-        The minimum integrated brightness. This is a crucial parameter for
-        eliminating spurious features.
-        Recommended minimum values are 100 for integer images and 1 for float
-        images. Defaults to 0 (no filtering).
-        .. warning:: The mass value is changed since v0.3.0
-        .. warning:: The default behaviour of minmass has changed since v0.4.0
-    maxsize : float
-        maximum radius-of-gyration of brightness, default None
-    separation : float or tuple
-        Minimum separation between features.
-        Default is diameter + 1. May be a tuple, see diameter for details.
-    noise_size : float or tuple
-        Width of Gaussian blurring kernel, in pixels
-        Default is 1. May be a tuple, see diameter for details.
-    smoothing_size : float or tuple
-        The size of the sides of the square kernel used in boxcar (rolling
-        average) smoothing, in pixels
-        Default is diameter. May be a tuple, making the kernel rectangular.
-    threshold : float
-        Clip bandpass result below this value. Thresholding is done on the
-        already background-subtracted image.
-        By default, 1 for integer images and 1/255 for float images.
-    invert : boolean
-        This will be deprecated. Use an appropriate PIMS pipeline to invert a
-        Frame or FramesSequence.
-        Set to True if features are darker than background. False by default.
-    percentile : float
-        Features must have a peak brighter than pixels in this
-        percentile. This helps eliminate spurious peaks.
-    topn : integer
-        Return only the N brightest features above minmass.
+    image : image array (any dimensions)
+    diameter : feature size in px
+    minmass : minimum integrated brightness
+        Default is 100, but a good value is often much higher. This is a
+        crucial parameter for elminating spurrious features.
+    maxsize : maximum radius-of-gyration of brightness, default None
+    separation : feature separation, in pixels
+        Default is the feature diameter + 1.
+    noise_size : width of Gaussian blurring kernel, in pixels
+        Default is 1.
+    smoothing_size : size of boxcar smoothing, in pixels
+        Default is the same is feature separation.
+    threshold : Clip bandpass result below this value.
+        Default None, passed through to bandpass.
+    invert : Set to True if features are darker than background. False by
+        default.
+    percentile : Features must have a peak brighter than pixels in this
+        percentile. This helps eliminate spurrious peaks.
+    topn : Return only the N brightest features above minmass.
         If None (default), return all features above minmass.
-    preprocess : boolean
-        Set to False to turn off bandpass preprocessing.
+
+    Returns
+    -------
+    DataFrame([x, y, mass, size, ecc, signal])
+        where mass means total integrated brightness of the blob,
+        size means the radius of gyration of its Gaussian-like profile,
+        and ecc is its eccentricity (1 is circular).
+
+    Other Parameters
+    ----------------
+    preprocess : Set to False to turn out bandpass preprocessing.
     max_iterations : integer
         max number of loops to refine the center of mass, default 10
     filter_before : boolean
-        filter_before is no longer supported as it does not improve performance.
+        Use minmass (and maxsize, if set) to eliminate spurrious features
+        based on their estimated mass and size before refining position.
+        True by default for performance.
     filter_after : boolean
-        This parameter has been deprecated: use minmass and maxsize.
+        Use final characterizations of mass and size to elminate spurrious
+        features. True by default.
     characterize : boolean
         Compute "extras": eccentricity, signal, ep. True by default.
     engine : {'auto', 'python', 'numba'}
 
-    Returns
-    -------
-    DataFrame([x, y, mass, size, ecc, signal, raw_mass])
-        where "x, y" are appropriate to the dimensionality of the image,
-        mass means total integrated brightness of the blob,
-        size means the radius of gyration of its Gaussian-like profile,
-        ecc is its eccentricity (0 is circular),
-        and raw_mass is the total integrated brightness in raw_image.
-
     See Also
     --------
     batch : performs location on many images in batch
-    minmass_v03_change : to convert minmass from v0.2.4 to v0.3.0
-    minmass_v04_change : to convert minmass from v0.3.x to v0.4.x
 
     Notes
     -----
-    Locate works with a coordinate system that has its origin at the center of
-    pixel (0, 0). In almost all cases this will be the top-left pixel: the
-    y-axis is pointing downwards.
-
     This is an implementation of the Crocker-Grier centroid-finding algorithm.
     [1]_
 
     References
     ----------
     .. [1] Crocker, J.C., Grier, D.G. http://dx.doi.org/10.1006/jcis.1996.0217
 
     """
-    if invert:
-        warnings.warn("The invert argument will be deprecated. Use a PIMS "
-                      "pipeline for this.", PendingDeprecationWarning)
-    if filter_before is not None:
-        raise ValueError("The filter_before argument is no longer supported as "
-                         "it does not improve performance. Features are "
-                         "filtered after refine.") # see GH issue #141
-    if filter_after is not None:
-        warnings.warn("The filter_after argument has been deprecated: it is "
-                      "always on, unless minmass = None and maxsize = None.",
-                      DeprecationWarning)
 
     # Validate parameters and set defaults.
-    raw_image = np.squeeze(raw_image)
-    shape = raw_image.shape
-    ndim = len(shape)
-
-    diameter = validate_tuple(diameter, ndim)
-    diameter = tuple([int(x) for x in diameter])
-    if not np.all([x & 1 for x in diameter]):
-        raise ValueError("Feature diameter must be an odd integer. Round up.")
-    radius = tuple([x//2 for x in diameter])
-
-    isotropic = np.all(radius[1:] == radius[:-1])
-    if (not isotropic) and (maxsize is not None):
-        raise ValueError("Filtering by size is not available for anisotropic "
-                         "features.")
-
-    is_float_image = not np.issubdtype(raw_image.dtype, np.integer)
-
-    if separation is None:
-        separation = tuple([x + 1 for x in diameter])
-    else:
-        separation = validate_tuple(separation, ndim)
-
+    if not diameter & 1:
+        raise ValueError("Feature diameter must be an odd number. Round up.")
+    if not separation:
+        separation = int(diameter) + 1
+    radius = int(diameter)//2
     if smoothing_size is None:
         smoothing_size = diameter
-    else:
-        smoothing_size = validate_tuple(smoothing_size, ndim)
-
-    noise_size = validate_tuple(noise_size, ndim)
-
-    if minmass is None:
-        minmass = 0
-
+    raw_image = np.squeeze(raw_image)
+    shape = raw_image.shape
     # Check whether the image looks suspiciously like a color image.
     if 3 in shape or 4 in shape:
         dim = raw_image.ndim
-        warnings.warn("I am interpreting the image as {}-dimensional. "
-                      "If it is actually a {}-dimensional color image, "
+        warnings.warn("I am interpreting the image as {0}-dimensional. "
+                      "If it is actually a {1}-dimensional color image, "
                       "convert it to grayscale first.".format(dim, dim-1))
-
-    if threshold is None:
-        if is_float_image:
-            threshold = 1/255.
-        else:
-            threshold = 1
-
-    # Invert the image if necessary
-    if invert:
-        raw_image = invert_image(raw_image)
-
-    # Determine `image`: the image to find the local maxima on.
     if preprocess:
+        if invert:
+            # It is tempting to do this in place, but if it is called multiple
+            # times on the same image, chaos reigns.
+            if np.issubdtype(raw_image.dtype, np.integer):
+                max_value = np.iinfo(raw_image.dtype).max
+                raw_image = raw_image ^ max_value
+            else:
+                # To avoid degrading performance, assume gamut is zero to one.
+                # Have you ever encountered an image of unnormalized floats?
+                raw_image = 1 - raw_image
         image = bandpass(raw_image, noise_size, smoothing_size, threshold)
     else:
-        image = raw_image
-
-    # For optimal performance, performance, coerce the image dtype to integer.
-    if is_float_image:  # For float images, assume bitdepth of 8.
-        dtype = np.uint8
-    else:   # For integer images, take original dtype
+        image = raw_image.copy()
+    # Coerce the image into integer type. Rescale to fill dynamic range.
+    if np.issubdtype(raw_image.dtype, np.integer):
         dtype = raw_image.dtype
-    # Normalize_to_int does nothing if image is already of integer type.
-    scale_factor, image = convert_to_int(image, dtype)
+    else:
+        dtype = np.int8
+    image = scale_to_gamut(image, dtype)
 
-    pos_columns = default_pos_columns(image.ndim)
+    # Set up a DataFrame for the final results.
+    if image.ndim < 4:
+        coord_columns = ['x', 'y', 'z'][:image.ndim]
+    else:
+        coord_columns = map(lambda i: 'x' + str(i), range(image.ndim))
+    char_columns = ['mass']
+    if characterize:
+        char_columns += ['size', 'ecc', 'signal']
+    columns = coord_columns + char_columns
+    # The 'ep' column is joined on at the end, so we need this...
+    if characterize:
+        all_columns = columns + ['ep']
+    else:
+        all_columns = columns
 
     # Find local maxima.
-    # Define zone of exclusion at edges of image, avoiding
-    #   - Features with incomplete image data ("radius")
-    #   - Extended particles that cannot be explored during subpixel
-    #       refinement ("separation")
-    #   - Invalid output of the bandpass step ("smoothing_size")
-    margin = tuple([max(rad, sep // 2 - 1, sm // 2) for (rad, sep, sm) in
-                    zip(radius, separation, smoothing_size)])
-    # Find features with minimum separation distance of `separation`. This
-    # excludes detection of small features close to large, bright features
-    # using the `maxsize` argument.
-    coords = grey_dilation(image, separation, percentile, margin, precise=False)
+    coords = local_maxima(image, radius, separation, percentile)
+    count_maxima = coords.shape[0]
+
+    if count_maxima == 0:
+        return DataFrame(columns=all_columns)
+
+    # Proactively filter based on estimated mass/size before
+    # refining positions.
+    if filter_before:
+        approx_mass = np.empty(count_maxima)  # initialize to avoid appending
+        for i in range(count_maxima):
+            approx_mass[i] = estimate_mass(image, radius, coords[i])
+        condition = approx_mass > minmass
+        if maxsize is not None:
+            approx_size = np.empty(count_maxima)
+            for i in range(count_maxima):
+                approx_size[i] = estimate_size(image, radius, coords[i],
+                                               approx_mass[i])
+            condition &= approx_size < maxsize
+        coords = coords[condition]
+    count_qualified = coords.shape[0]
+
+    if count_qualified == 0:
+        warnings.warn("No maxima survived mass- and size-based prefiltering.")
+        return DataFrame(columns=all_columns)
 
     # Refine their locations and characterize mass, size, etc.
-    refined_coords = refine_com(raw_image, image, radius, coords,
-                                max_iterations=max_iterations,
-                                engine=engine, characterize=characterize)
-    if len(refined_coords) == 0:
-        return refined_coords
+    refined_coords = refine(raw_image, image, radius, coords, max_iterations,
+                            engine, characterize)
 
-    # Flat peaks return multiple nearby maxima. Eliminate duplicates.
-    if np.all(np.greater(separation, 0)):
-        to_drop = where_close(refined_coords[pos_columns], separation,
-                              refined_coords['mass'])
-        refined_coords.drop(to_drop, axis=0, inplace=True)
-        refined_coords.reset_index(drop=True, inplace=True)
-
-    # mass and signal values has to be corrected due to the rescaling
-    # raw_mass was obtained from raw image; size and ecc are scale-independent
-    refined_coords['mass'] /= scale_factor
-    if 'signal' in refined_coords:
-        refined_coords['signal'] /= scale_factor
-
-    # Filter on mass and size, if set.
-    condition = refined_coords['mass'] > minmass
-    if maxsize is not None:
-        condition &= refined_coords['size'] < maxsize
-    if not condition.all():  # apply the filter
-        # making a copy to avoid SettingWithCopyWarning
-        refined_coords = refined_coords.loc[condition].copy()
-
-    if len(refined_coords) == 0:
-        warnings.warn("No maxima survived mass- and size-based filtering. "
-                      "Be advised that the mass computation was changed from "
-                      "version 0.2.4 to 0.3.0 and from 0.3.3 to 0.4.0. "
-                      "See the documentation and the convenience functions "
-                      "'minmass_v03_change' and 'minmass_v04_change'.")
-        return refined_coords
-
-    if topn is not None and len(refined_coords) > topn:
-        # go through numpy for easy pandas backwards compatibility
-        mass = refined_coords['mass'].values
+    # Filter again, using final ("exact") mass -- and size, if set.
+    MASS_COLUMN_INDEX = image.ndim
+    SIZE_COLUMN_INDEX = image.ndim + 1
+    exact_mass = refined_coords[:, MASS_COLUMN_INDEX]
+    if filter_after:
+        condition = exact_mass > minmass
+        if maxsize is not None:
+            exact_size = refined_coords[:, SIZE_COLUMN_INDEX]
+            condition &= exact_size < maxsize
+        refined_coords = refined_coords[condition]
+        exact_mass = exact_mass[condition]  # used below by topn
+    count_qualified = refined_coords.shape[0]
+
+    if count_qualified == 0:
+        warnings.warn("No maxima survived mass- and size-based filtering.")
+        return DataFrame(columns=all_columns)
+
+    if topn is not None and count_qualified > topn:
         if topn == 1:
             # special case for high performance and correct shape
-            refined_coords = refined_coords.iloc[[np.argmax(mass)]]
+            refined_coords = refined_coords[np.argmax(exact_mass)]
+            refined_coords = refined_coords.reshape(1, -1)
         else:
-            refined_coords = refined_coords.iloc[np.argsort(mass)[-topn:]]
+            refined_coords = refined_coords[np.argsort(exact_mass)][-topn:]
+
+    f = DataFrame(refined_coords, columns=columns)
 
     # Estimate the uncertainty in position using signal (measured in refine)
     # and noise (measured here below).
     if characterize:
-        black_level, noise = measure_noise(image, raw_image, radius)
-        Npx = N_binary_mask(radius, ndim)
-        mass = refined_coords['raw_mass'].values - Npx * black_level
-        ep = _static_error(mass, noise, radius, noise_size)
-
-        if ep.ndim == 1:
-            refined_coords['ep'] = ep
-        else:
-            ep = pd.DataFrame(ep, columns=['ep_' + cc for cc in pos_columns])
-            refined_coords = pandas_concat([refined_coords, ep], axis=1)
+        black_level, noise = uncertainty.measure_noise(
+            raw_image, diameter, threshold)
+        f['signal'] -= black_level
+        ep = uncertainty.static_error(f, noise, diameter, noise_size)
+        f = f.join(ep)
 
     # If this is a pims Frame object, it has a frame number.
     # Tag it on; this is helpful for parallelization.
     if hasattr(raw_image, 'frame_no') and raw_image.frame_no is not None:
-        refined_coords['frame'] = int(raw_image.frame_no)
-    return refined_coords
+        f['frame'] = raw_image.frame_no
+    return f
 
 
-def batch(frames, diameter, output=None, meta=None, processes='auto',
-          after_locate=None, **kwargs):
-    """Locate Gaussian-like blobs of some approximate size in a set of images.
+def batch(frames, diameter, minmass=100, maxsize=None, separation=None,
+          noise_size=1, smoothing_size=None, threshold=None, invert=False,
+          percentile=64, topn=None, preprocess=True, max_iterations=10,
+          filter_before=True, filter_after=True,
+          characterize=True, engine='auto',
+          output=None, meta=True):
+    """Locate Gaussian-like blobs of a given approximate size.
 
     Preprocess the image by performing a band pass and a threshold.
     Locate all peaks of brightness, characterize the neighborhoods of the peaks
-    and take only those with given total brightness ("mass"). Finally,
+    and take only those with given total brightnesss ("mass"). Finally,
     refine the positions of each peak.
 
     Parameters
     ----------
     frames : list (or iterable) of images
-        The frames to process.
-    diameter : odd integer or tuple of odd integers
-        This may be a single number or a tuple giving the feature's
-        extent in each dimension, useful when the dimensions do not have
-        equal resolution (e.g. confocal microscopy). The tuple order is the
-        same as the image shape, conventionally (z, y, x) or (y, x). The
-        number(s) must be odd integers. When in doubt, round up.
-    output : {None, trackpy.PandasHDFStore, SomeCustomClass}
-        If None, return all results as one big DataFrame. Otherwise, pass
-        results from each frame, one at a time, to the put() method
-        of whatever class is specified here.
-    meta : filepath or file object
-        If specified, information relevant to reproducing this batch is saved
-        as a YAML file, a plain-text machine- and human-readable format.
-        By default, this is None, and no file is saved.
-    processes : integer or "auto"
-        The number of processes to use in parallel. If <= 1, multiprocessing is
-        disabled. If "auto", the number returned by `os.cpu_count()`` is used.
-    after_locate : function
-        Specify a custom function to apply to the detected features in each
-        processed frame. It must accept the following arguments:
-
-        - ``frame_no``: an integer specifying the number of the current frame.
-        - ``features``: a DataFrame containing the detected features.
-
-        Furthermore it must return a DataFrame like ``features``.
-    **kwargs :
-        Keyword arguments that are passed to the wrapped `trackpy.locate`.
-        Refer to its docstring for further details.
+    diameter : feature size in px
+    minmass : minimum integrated brightness
+        Default is 100, but a good value is often much higher. This is a
+        crucial parameter for elminating spurrious features.
+    maxsize : maximum radius-of-gyration of brightness, default None
+    separation : feature separation, in pixels
+        Default is the feature diameter + 1.
+    noise_size : width of Gaussian blurring kernel, in pixels
+        Default is 1.
+    smoothing_size : size of boxcar smoothing, in pixels
+        Default is the same is feature separation.
+    threshold : Clip bandpass result below this value.
+        Default None, passed through to bandpass.
+    invert : Set to True if features are darker than background. False by
+        default.
+    percentile : Features must have a peak brighter than pixels in this
+        percentile. This helps eliminate spurrious peaks.
+    topn : Return only the N brightest features above minmass.
+        If None (default), return all features above minmass.
 
     Returns
     -------
     DataFrame([x, y, mass, size, ecc, signal])
         where mass means total integrated brightness of the blob,
         size means the radius of gyration of its Gaussian-like profile,
-        and ecc is its eccentricity (0 is circular).
+        and ecc is its eccentricity (1 is circular).
+
+    Other Parameters
+    ----------------
+    preprocess : Set to False to turn off bandpass preprocessing.
+    max_iterations : integer
+        max number of loops to refine the center of mass, default 10
+    filter_before : boolean
+        Use minmass (and maxsize, if set) to eliminate spurrious features
+        based on their estimated mass and size before refining position.
+        True by default for performance.
+    filter_after : boolean
+        Use final characterizations of mass and size to elminate spurrious
+        features. True by default.
+    characterize : boolean
+        Compute "extras": eccentricity, signal, ep. True by default.
+    engine : {'auto', 'python', 'numba'}
+    output : {None, trackpy.PandasHDFStore, SomeCustomClass}
+        If None, return all results as one big DataFrame. Otherwise, pass
+        results from each frame, one at a time, to the write() method
+        of whatever class is specified here.
+    meta : By default, a YAML (plain text) log file is saved in the current
+        directory. You can specify a different filepath set False.
 
     See Also
     --------
     locate : performs location on a single image
 
     Notes
     -----
-    This is a convenience function that wraps `trackpy.locate` (see its
-    docstring for further details) and allows batch processing of multiple
-    frames, optionally in parallel by using multiprocessing.
+    This is an implementation of the Crocker-Grier centroid-finding algorithm.
+    [1]_
+
+    References
+    ----------
+    .. [1] Crocker, J.C., Grier, D.G. http://dx.doi.org/10.1006/jcis.1996.0217
+
     """
-    if "raw_image" in kwargs:
-        raise KeyError("the argument `raw_image` musn't be in `kwargs`, it is "
-                       "provided internally by `frames`")
-    # Add required keyword argument
-    kwargs["diameter"] = diameter
+    # Gather meta information and save as YAML in current directory.
+    timestamp = pd.datetime.utcnow().strftime('%Y-%m-%d-%H%M%S')
+    try:
+        source = frames.filename
+    except:
+        source = None
+    meta_info = dict(timestamp=timestamp,
+                     trackpy_version=trackpy.__version__,
+                     source=source, diameter=diameter, minmass=minmass,
+                     maxsize=maxsize, separation=separation,
+                     noise_size=noise_size, smoothing_size=smoothing_size,
+                     invert=invert, percentile=percentile, topn=topn,
+                     preprocess=preprocess, max_iterations=max_iterations,
+                     filter_before=filter_before, filter_after=filter_after)
 
     if meta:
-        # Gather meta information and save as YAML in current directory.
-        try:
-            source = frames.filename
-        except AttributeError:
-            source = None
-        meta_info = dict(
-            timestamp=pd.datetime.utcnow().strftime('%Y-%m-%d-%H%M%S'),
-            trackpy_version=trackpy.__version__,
-            source=source,
-            **kwargs
-        )
         if isinstance(meta, str):
-            with open(meta, 'w') as file_obj:
-                record_meta(meta_info, file_obj)
+            filename = meta
         else:
-            # Interpret meta to be a file handle.
-            record_meta(meta_info, meta)
-
-    # Prepare wrapped function for mapping to `frames`
-    curried_locate = partial(locate, **kwargs)
-
-    pool, map_func = get_pool(processes)
+            filename = 'feature_log_%s.yml' % timestamp
+        record_meta(meta_info, filename)
 
-    if after_locate is None:
-        def after_locate(frame_no, features):
-            return features
+    all_features = []
+    for i, image in enumerate(frames):
+        features = locate(image, diameter, minmass, maxsize, separation,
+                          noise_size, smoothing_size, threshold, invert,
+                          percentile, topn, preprocess, max_iterations,
+                          filter_before, filter_after, characterize,
+                          engine)
+        if hasattr(image, 'frame_no') and image.frame_no is not None:
+            frame_no = image.frame_no
+            # If this works, locate created a 'frame' column.
+        else:
+            frame_no = i
+            features['frame'] = i  # just counting iterations
+        message = "Frame %d: %d features" % (frame_no, len(features))
+        print_update(message)
+        if len(features) == 0:
+            continue
 
-    try:
-        all_features = []
-        for i, features in enumerate(map_func(curried_locate, frames)):
-            image = frames[i]
-            if hasattr(image, 'frame_no') and image.frame_no is not None:
-                frame_no = image.frame_no
-                # Even if this worked, if locate() was running in parallel,
-                # it may not have had access to the "frame_no" attribute.
-                # Therefore we'll add the frame number to the DataFrame if
-                # needed, below.
-            else:
-                frame_no = i
-            if 'frame' not in features.columns:
-                features['frame'] = frame_no  # just counting iterations
-            features = after_locate(frame_no, features)
-
-            logger.info("Frame %d: %d features", frame_no, len(features))
-            if len(features) > 0:
-                # Store if features were found
-                if output is None:
-                    all_features.append(features)
-                else:
-                    output.put(features)
-    finally:
-        if pool:
-            # Ensure correct termination of Pool
-            pool.terminate()
+        if output is None:
+            all_features.append(features)
+        else:
+            output.put(features)
 
     if output is None:
-        if len(all_features) > 0:
-            return pandas_concat(all_features).reset_index(drop=True)
-        else:  # return empty DataFrame
-            warnings.warn("No maxima found in any frame.")
-            return pd.DataFrame(columns=list(features.columns) + ['frame'])
+        return pd.concat(all_features).reset_index(drop=True)
     else:
         return output
-
-
-def characterize(coords, image, radius, scale_factor=1.):
-    """ Characterize a 2d ndarray of coordinates. Returns a dictionary of 1d
-    ndarrays. If the feature region (partly) falls out of the image, then the
-    corresponding element in the characterized arrays will be NaN."""
-    shape = image.shape
-    N, ndim = coords.shape
-
-    radius = validate_tuple(radius, ndim)
-    isotropic = is_isotropic(radius)
-
-    # largely based on trackpy.refine.center_of_mass._refine
-    coords_i = np.round(coords).astype(int)
-    mass = np.full(N, np.nan)
-    signal = np.full(N, np.nan)
-    ecc = np.full(N, np.nan)
-
-    mask = binary_mask(radius, ndim).astype(np.uint8)
-    if isotropic:
-        Rg = np.full(len(coords), np.nan)
-    else:
-        Rg = np.full((len(coords), len(radius)), np.nan)
-
-    for feat, coord in enumerate(coords_i):
-        if np.any([c - r < 0 or c + r >= sh
-                   for c, r, sh in zip(coord, radius, shape)]):
-            continue
-        rect = [slice(c - r, c + r + 1) for c, r in zip(coord, radius)]
-        neighborhood = mask * image[tuple(rect)]
-        mass[feat] = neighborhood.sum() / scale_factor
-        signal[feat] = neighborhood.max() / scale_factor
-        if isotropic:
-            Rg[feat] = np.sqrt(np.sum(r_squared_mask(radius, ndim) *
-                                      neighborhood) / mass[feat])
-        else:
-            Rg[feat] = np.sqrt(ndim * np.sum(x_squared_masks(radius, ndim) *
-                                             neighborhood,
-                                             axis=tuple(range(1, ndim + 1))) /
-                               mass[feat])[::-1]  # change order yx -> xy
-        # I only know how to measure eccentricity in 2D.
-        if ndim == 2:
-            ecc[feat] = np.sqrt(np.sum(neighborhood*cosmask(radius))**2 +
-                                np.sum(neighborhood*sinmask(radius))**2)
-            ecc[feat] /= (mass[feat] - neighborhood[radius] + 1e-6)
-
-    result = dict(mass=mass, signal=signal, ecc=ecc)
-    if isotropic:
-        result['size'] = Rg
-    else:
-        for _size, key in zip(Rg.T, default_size_columns(ndim, isotropic)):
-            result[key] = _size
-    return result
```

### Comparing `trackpy-0.6.3rc1/trackpy/filtering.py` & `trackpy-unknown/trackpy/filtering.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,38 @@
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
+
 """Simple functions that eliminate spurrious trajectories
 by wrapping pandas group-by and filter capabilities."""
 
-__all__ = ['filter_stubs', 'filter_clusters', 'filter']
-
 
 def filter_stubs(tracks, threshold=100):
-    """Filter out trajectories with few points. They are often spurious.
+    """Filter out trajectories with few points. They are often specious.
 
     Parameters
     ----------
     tracks : DataFrame
         must include columns named 'frame' and 'particle'
     threshold : integer, default 100
-        minimum number of points (video frames) to survive
+        minimum number of points to survive
 
     Returns
     -------
     a subset of tracks
     """
     try:
         tracks['frame']
         tracks['particle']
     except KeyError:
         raise ValueError("Tracks must contain columns 'frame' and 'particle'.")
     grouped = tracks.reset_index(drop=True).groupby('particle')
     filtered = grouped.filter(lambda x: x.frame.count() >= threshold)
     return filtered.set_index('frame', drop=False)
 
-
 def filter_clusters(tracks, quantile=0.8, threshold=None):
     """Filter out trajectories with a mean particle size above a given quantile.
 
     Parameters
     ----------
     tracks : DataFrame
         must include columns named 'particle' and 'size'
@@ -48,15 +49,15 @@
         tracks['frame']
         tracks['particle']
     except KeyError:
         raise ValueError("Tracks must contain columns 'frame' and 'particle'.")
     if threshold is None:
         threshold = tracks['size'].quantile(quantile)
 
-    f = lambda x: x['size'].mean() < threshold  # filtering function
+    f = lambda x: x['size'].mean() < threshold # filtering function
     grouped = tracks.reset_index(drop=True).groupby('particle')
     filtered = grouped.filter(f)
     return filtered.set_index('frame', drop=False)
 
 
 def filter(tracks, condition_func):
     """A workaround for a bug in pandas 0.12
```

### Comparing `trackpy-0.6.3rc1/trackpy/framewise_data.py` & `trackpy-unknown/trackpy/framewise_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import logging
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
 import os
 from abc import ABCMeta, abstractmethod, abstractproperty
-import warnings
 
 import pandas as pd
 
-from .utils import pandas_concat
+from .utils import print_update
 
-logger = logging.getLogger(__name__)
 
-
-class FramewiseData:
-    "Abstract base class defining a data container with framewise access."
+class FramewiseData(object):
 
     __metaclass__ = ABCMeta
 
     @abstractmethod
     def put(self, df):
         pass
 
@@ -50,27 +48,27 @@
             optional; if None, return all frames
 
         Returns
         -------
         DataFrame
         """
         if N is None:
-            return pandas_concat(iter(self))
+            return pd.concat(iter(self))
         else:
             i = iter(self)
-            return pandas_concat(next(i) for _ in range(N))
+            return pd.concat((next(i) for _ in range(N)))
 
     @property
     def max_frame(self):
         return max(self.frames)
 
     def _validate(self, df):
         if self.t_column not in df.columns:
             raise ValueError("Cannot write frame without a column "
-                             "called {}".format(self.t_column))
+                             "called {0}".format(self.t_column))
         if df[self.t_column].nunique() != 1:
             raise ValueError("Found multiple values for 'frame'. "
                              "Write one frame at a time.")
 
     def __iter__(self):
         return self._build_generator()
 
@@ -86,27 +84,25 @@
 
 KEY_PREFIX = 'Frame_'
 len_key_prefix = len(KEY_PREFIX)
 
 
 def code_key(frame_no):
     "Turn the frame_no into a 'natural name' string idiomatic of HDFStore"
-    key = '{}{}'.format(KEY_PREFIX, frame_no)
+    key = '{0}{1}'.format(KEY_PREFIX, frame_no)
     return key
 
 
 def decode_key(key):
     frame_no = int(key[len_key_prefix:])
     return frame_no
 
 
 class PandasHDFStore(FramewiseData):
-    """An interface to an HDF5 file with framewise access, using pandas.
-
-    Save each frame's data to a node in a pandas HDFStore.
+    """Save each frame's data to a node in a pandas HDFStore.
 
     Any additional keyword arguments to the constructor are passed to
     pandas.HDFStore().
     """
 
     def __init__(self, filename, mode='a', t_column='frame', **kwargs):
         self.filename = os.path.abspath(filename)
@@ -118,17 +114,14 @@
         return self._t_column
 
     @property
     def max_frame(self):
         return max(self.frames)
 
     def put(self, df):
-        if len(df) == 0:
-            warnings.warn('An empty DataFrame was passed to put(). Continuing.')
-            return
         frame_no = df[self.t_column].values[0]  # validated to be all the same
         key = code_key(frame_no)
         # Store data as tabular instead of fixed-format.
         # Make sure remove any prexisting data, so don't really 'append'.
         try:
             self.store.remove(key)
         except KeyError:
@@ -155,15 +148,14 @@
              key.startswith(KEY_PREFIX)]
         r.sort()
         return r
 
     def close(self):
         self.store.close()
 
-
 class PandasHDFStoreBig(PandasHDFStore):
     """Like PandasHDFStore, but keeps a cache of frame numbers.
 
     This can give a large performance boost when a file contains thousands
     of frames.
 
     If a file was made in PandasHDFStore, opening it with this class
@@ -173,15 +165,15 @@
     pandas.HDFStore().
     """
 
     def __init__(self, filename, mode='a', t_column='frame', **kwargs):
         self._CACHE_NAME = '_Frames_Cache'
         self._frames_cache = None
         self._cache_dirty = False  # Whether _frames_cache needs to be written out
-        super().__init__(filename, mode, t_column,
+        super(PandasHDFStoreBig, self).__init__(filename, mode, t_column,
                                                 **kwargs)
 
     @property
     def frames(self):
         # Hit memory cache, then disk cache
         if self._frames_cache is not None:
             return self._frames_cache
@@ -192,15 +184,15 @@
             except KeyError:
                 self._frames_cache = self._get_frame_nos()
                 self._cache_dirty = True # In memory, but not in file
             return self._frames_cache
 
     def put(self, df):
         self._invalidate_cache()
-        super().put(df)
+        super(PandasHDFStoreBig, self).put(df)
 
     def rebuild_cache(self):
         """Delete cache on disk and rebuild it."""
         self._invalidate_cache()
         _ = self.frames # Compute cache
         self._flush_cache()
 
@@ -219,20 +211,19 @@
             self._cache_dirty = False
 
     def close(self):
         """Updates cache, writes if necessary, then closes file."""
         if self.store.root._v_file._iswritable():
             _ = self.frames # Compute cache
             self._flush_cache()
-        super().close()
+        super(PandasHDFStoreBig, self).close()
 
 
 class PandasHDFStoreSingleNode(FramewiseData):
-    """An interface to an HDF5 file with framewise access,
-    using pandas, that is faster for cross-frame queries.
+    """Save all frames into one large node.
 
     This implementation is more complex than PandasHDFStore,
     but it simplifies (speeds up?) cross-frame queries,
     like queries for a single probe's entire trajectory.
 
     Any additional keyword arguments to the constructor are passed to
     pandas.HDFStore().
@@ -241,36 +232,32 @@
     def __init__(self, filename, key='FrameData', mode='a', t_column='frame',
                  use_tabular_copy=False, **kwargs):
         self.filename = os.path.abspath(filename)
         self.key = key
         self._t_column = t_column
         self.store = pd.HDFStore(self.filename, mode, **kwargs)
 
-        store = pd.HDFStore(self.filename)
-        try:
-            store[self.key]
-        except KeyError:
-            pass
-        else:
-            self._validate_node(use_tabular_copy)
-        store.close()
+        with pd.get_store(self.filename) as store:
+            try:
+                store[self.key]
+            except KeyError:
+                pass
+            else:
+                self._validate_node(use_tabular_copy)
 
     @property
     def t_column(self):
         return self._t_column
 
     def put(self, df):
-        if len(df) == 0:
-            warnings.warn('An empty DataFrame was passed to put(). Continuing.')
-            return
         self._validate(df)
         self.store.append(self.key, df, data_columns=True)
 
     def get(self, frame_no):
-        frame = self.store.select(self.key, '{} == {}'.format(
+        frame = self.store.select(self.key, '{0} == {1}'.format(
             self._t_column, frame_no))
         return frame
 
     def dump(self, N=None):
         """Return data from all, or the first N, frames in a single DataFrame
 
         Parameters
@@ -282,15 +269,15 @@
         -------
         DataFrame
         """
         if N is None:
             return self.store.select(self.key)
         else:
             Nth_frame = self.frames[N - 1]
-            return self.store.select(self.key, '{} <= {}'.format(
+            return self.store.select(self.key, '{0} <= {1}'.format(
                 self._t_column, Nth_frame))
 
     def close(self):
         self.store.close()
 
     def __del__(self):
         if hasattr(self, 'store'):
@@ -302,28 +289,28 @@
         # I assume one column can fit in memory, which is not ideal.
         # Chunking does not seem to be implemented for select_column.
         frame_nos = self.store.select_column(self.key, self.t_column).unique()
         frame_nos.sort()
         return frame_nos
 
     def _validate_node(self, use_tabular_copy):
-        # The HDFStore might be non-tabular, which means we cannot select a
+        # The HDFStore might be non-tabular, which means we cannot select a 
         # subset, and this whole structure will not work.
         # For convenience, this can rewrite the table into a tabular node.
         if use_tabular_copy:
             self.key = _make_tabular_copy(self.filename, self.key)
 
         pandas_type = getattr(getattr(getattr(
-            self.store._handle.root, self.key, None), '_v_attrs', None),
+            self.store._handle.root, self.key, None), '_v_attrs', None), 
             'pandas_type', None)
         if not pandas_type == 'frame_table':
             raise ValueError("This node is not tabular. Call with "
                              "use_tabular_copy=True to proceed.")
 
 
 def _make_tabular_copy(store, key):
     """Copy the contents nontabular node in a pandas HDFStore
     into a tabular node"""
     tabular_key = key + '/tabular'
-    logger.info("Making a tabular copy of %s at %s", (key, tabular_key))
+    print_update("Making a tabular copy of %s at %s" % (key, tabular_key))
     store.append(tabular_key, store.get(key), data_columns=True)
     return tabular_key
```

### Comparing `trackpy-0.6.3rc1/trackpy/linking/legacy.py` & `trackpy-unknown/trackpy/linking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,179 @@
-import logging
-from warnings import warn
-import itertools
-import functools
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
+from six.moves import zip, range
+from copy import copy
+import itertools, functools
+from collections import deque, Iterable
 
 import numpy as np
-import pandas as pd
 from scipy.spatial import cKDTree
+import pandas as pd
 
-from ..try_numba import NUMBA_AVAILABLE
-from ..utils import pandas_sort, validate_tuple, is_isotropic
-from .utils import (TrackUnstored, points_to_arr, UnknownLinkingError,
-                    SubnetOversizeException)
-from .subnetlinker import (recursive_linker_obj, nonrecursive_link, drop_link,
-                           numba_link)
+from .utils import print_update
+from .try_numba import try_numba_autojit, NUMBA_AVAILABLE
 
-logger = logging.getLogger(__name__)
+class TreeFinder(object):
 
+    def __init__(self, points):
+        """Takes a list of particles.
+        """
+        self.points = copy(points)
+        self.rebuild()
 
-class Point:
-    '''
-    Base class for point (features) used in tracking.  This class
-    contains all of the general stuff for interacting with
-    :py:class:`~trackpy.linking.Track` objects.
+    def add_point(self, pt):
+        self.points.append(pt)
+        self._clean = False
 
+    def rebuild(self, coord_map=None):
+        """Rebuilds tree from ``points`` attribute.
 
-    .. note:: To be used for tracking this class must be sub-classed to provide
-    a :py:meth:`distance` function.  Child classes **MUST** call
-    :py:meth:`Point.__init__`.  (See :py:class:`~trackpy.linking.PointND` for
-    example. )
-    '''
-    @classmethod
-    def reset_counter(cls, c=0):
-        cls.counter = itertools.count(c)
+        coord_map : function (optional)
+            Called with a list of N Point instances, returns their "effective" locations,
+            as an N x d array (or list of tuples). Used for prediction (see "predict" module).
 
-    def __init__(self):
-        self._track = None
-        self.uuid = next(self.counter)         # unique id for __hash__
+        rebuild() needs to be called after ``add_point()`` and before tree is used for
+        spatial queries again (i.e. when memory is turned on).
+        """
 
-    # def __eq__(self, other):
-    #     return self.uuid == other.uuid
+        if coord_map is None:
+            coord_map = functools.partial(map, lambda x: x.pos)
+        coords = np.asarray(list(coord_map(self.points)))
+        if len(self.points) == 0:
+            raise ValueError('Frame (aka level) contains zero points')
+        self._kdtree = cKDTree(coords, 15)
+        # This could be tuned
+        self._clean = True
 
-    # def __neq__(self, other):
-    #     return not self.__eq__(other)
+    @property
+    def kdtree(self):
+        if not self._clean:
+            self.rebuild()
+        return self._kdtree
 
-    def add_to_track(self, track):
-        '''
-        :param track: the track to assign to this :py:class:`Point`
 
-        Sets the track of a :py:class:`Point` object.  Raises
-        :py:exc:`Exception` if the object is already assigned a track.
+class HashTable(object):
+    '''
+    :param dims: the range of the data to be put in the hash table.  0<data[k]<dims[k]
+    :param box_size: how big each box should be in data units.  The same scale is used for all dimensions
 
+    Basic hash table to fast look up of particles in the region of a given particle
+    '''
+    class Out_of_hash_excpt(Exception):
+        """
+        :py:exc:`Exception` for indicating that a particle is outside of the
+        valid range for this hash table."""
+        pass
 
+    def __init__(self, dims, box_size):
+        '''
+        Sets up the hash table
 
         '''
-        if self._track is not None:
-            raise Exception("trying to add a particle already in a track")
-        self._track = track
+        self.dims = dims                  # the dimensions of the data
+        self.box_size = box_size          # the size of boxes to use in the units of the data
+        self.hash_dims = np.ceil(np.array(dims) / box_size)
 
-    def remove_from_track(self, track):
+        self.hash_table = [[] for j in range(int(np.prod(self.hash_dims)))]
+        self.spat_dims = len(dims)        # how many spatial dimensions
+        self.cached_shifts = None
+        self.cached_rrange = None
+        self.strides = np.cumprod(np.concatenate(([1], self.hash_dims[1:])))[::-1]
+
+    def get_region(self, point, rrange):
         '''
-        :param track: the track to disassociate from this :py:class:`Point`
+        :param point: point to find the features around
+        :param rrange: the size of the ball to search in
 
-        Removes this point from the given track. Raises :py:exc:`Exception` if
-        particle not associated with the given track.
 
+        Returns all the particles with in the region of maximum radius
+        rrange in data units
 
-        '''
-        if self._track != track:
-            raise Exception("Point not associated with given track")
-        track.remove_point(self)
 
-    def in_track(self):
+        can raise :py:exc:`Out_of_hash_excpt`
         '''
-        :rtype: bool
+        hash_size = self.hash_dims
+        center = np.floor(point.pos / self.box_size)
+        if any(center >= hash_size) or any(center < 0):
+            raise Hash_table.Out_of_hash_excpt("cord out of range")
+
+        rrange = int(np.ceil(rrange / self.box_size))
+
+        # check if we have already computed the shifts
+        if rrange == self.cached_rrange and self.cached_shifts is not None:
+            shifts = self.cached_shifts   # if we have, use them
+        # Other wise, generate them
+        else:
+            if self.spat_dims == 2:
+                shifts = [np.array([j, k])
+                          for j in range(-rrange, rrange + 1)
+                          for k in range(-rrange, rrange + 1)]
+            elif self.spat_dims == 3:
+                shifts = [np.array([j, k, m])
+                          for j in range(-rrange, rrange + 1)
+                          for k in range(-rrange, rrange + 1)
+                          for m in range(-rrange, rrange + 1)]
+            else:
+                raise NotImplementedError('only 2 and 3 dimensions implemented')
+            self.cached_rrange = rrange   # and save them
+            self.cached_shifts = shifts
+        region = []
+
+        for s in shifts:
+
+            cord = center + s
+            if any(cord >= hash_size) or any(cord < 0):
+                continue
+            indx = int(sum(cord * self.strides))
+            region.extend(self.hash_table[indx])
+        return region
+
+    def add_point(self, point):
+        """
+        :param point: object representing the feature to add to the hash table
+
+        Adds the `point` to the hash table.  Assumes that :py:attr:`point.pos` exists and
+        is the array-like.
+
 
-        Returns if a point is associated with a track '''
-        return self._track is not None
 
-    @property
-    def track(self):
-        """Returns the track that this :class:`Point` is in.  May be `None` """
-        return self._track
 
+        can raise :py:exc:`~Hash_table.Out_of_hash_excpt`
 
-class Track(TrackUnstored):
+        """
+        cord = np.floor(np.asarray(point.pos) / self.box_size)
+        hash_size = self.hash_dims
+        if any(cord >= hash_size) or any(cord < 0):
+            raise Hash_table.Out_of_hash_excpt("cord out of range")
+        indx = int(sum(cord * self.strides))
+        self.hash_table[indx].append(point)
+
+
+class Track(object):
     '''
-    Base class for objects to represent linked tracks.
+    :param point: The first feature in the track if not  `None`.
+    :type point: :py:class:`~trackpy.tracking.Point`
 
-    Includes logic for adding, removing features to the track.  This can
-    be sub-classed to provide additional track level computation as
-    needed.
+    Base class for objects to represent linked tracks.  Includes logic
+    for adding, removing features to the track.  This can be sub-classed
+    to provide additional track level computation as needed.
 
-    Parameters
-    ----------
-    point : Point or None, optional
-        The first feature in the track
 
     '''
+    count = 0
+
     def __init__(self, point=None):
         self.points = []
-        super().__init__(point)
+        # will take initiator point
+        if not point is None:
+            self.add_point(point)
+
+        self.indx = Track.count           # unique id
+        Track.count += 1
 
     def __iter__(self):
         return self.points.__iter__()
 
     def __len__(self):
         return len(self.points)
 
@@ -113,315 +183,203 @@
     def __neq__(self, other):
         return not self.__eq__(other)
     __hash__ = None
 
     def add_point(self, point):
         '''
         :param point: point to add
-        :type point:  :py:class:`~trackpy.linking.Point`
+        :type point:  :py:class:`~trackpy.tracking.Point`
 
         Appends the point to this track. '''
         self.points.append(point)
         point.add_to_track(self)
 
     def remove_point(self, point):
         '''
         :param point: point to remove from this track
-        :type point:  :py:class:`~trackpy.linking.Point`
+        :type point:  :py:class:`~trackpy.tracking.Point`
 
         removes a point from this track'''
         self.points.remove(point)
         point._track = None
 
     def last_point(self):
         '''
-        :rtype: :py:class:`~trackpy.linking.Point`
+        :rtype: :py:class:`~trackpy.tracking.Point`
 
         Returns the last point on the track'''
         return self.points[-1]
 
+    def __repr__(self):
+        return "<%s %d>" % (self.__class__.__name__, self.indx)
 
-class PointND(Point):
-    '''
-    Version of :class:`Point` for tracking in flat space with
-    non-periodic boundary conditions.
-
-    Parameters
-    ----------
-    t : scalar
-        a time-like variable.
-
-    pos : array-like
-        position of feature
-
-    id : int, optional
-        external unique ID
-    '''
-
-    def __init__(self, t, pos, id=None):
-        Point.__init__(self)                  # initialize base class
-        self.t = t                            # time
-        self.pos = np.asarray(pos)            # position in ND space
-        self.id = id
-
-    def distance(self, other_point):
-        '''
-        :param other_point: point to get distance to.
-        :type other_point: :py:class:`~trackpy.linking.Point`
+    @classmethod
+    def reset_counter(cls, c=0):
+        cls.count = 0
 
-        Returns the absolute distance between this point and other_point
 
-        '''
-        return np.sqrt(np.sum((self.pos - other_point.pos) ** 2))
+class DummyTrack(object):
+    "Does not store points, thereby conserving memory."
 
-    def __str__(self):
-        return "({t}, {p})".format(t=self.t, p=self.pos)
+    track_id = itertools.count(0)
 
-    def __repr__(self):
-        coords = '(' + (', '.join(["{:.3f}"]*len(self.pos))).format(*self.pos) + ')'
-        track = " in Track %d" % self.track.indx if self.track else ""
-        return "<%s at %d, " % (self.__class__.__name__, self.t) + coords + track + ">"
+    def __init__(self, point):
+       self.id = next(DummyTrack.track_id)
+       self.indx = self.id  # redundant, but like trackpy
+       if point is not None:
+           self.add_point(point)
 
+    def add_point(self, point):
+        point.add_to_track(self)
 
-class PointDiagnostics:
-    """Mixin to add memory diagnostics collection to a Point object."""
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.diag = {}
+    @classmethod
+    def reset_counter(cls, c=0):
+        cls.track_id = itertools.count(c)
 
-    def add_to_track(self, track):
-        super().add_to_track(track)
-        # See the note in the memory section of Linker.link(). If this link
-        # is from memory, the track knows how many frames were skipped.
-        memcount = track.report_memory()
-        if memcount > 0:
-            self.diag['remembered'] = memcount
-
-class PointNDDiagnostics(PointDiagnostics, PointND):
-    """Version of :class:`PointND` that collects diagnostic information
-    during tracking.
-    """
-    pass
 
+class Point(object):
+    '''
+    Base class for point (features) used in tracking.  This class
+    contains all of the general stuff for interacting with
+    :py:class:`~trackpy.tracking.Track` objects.
 
-class TreeFinder:
-    def __init__(self, points, search_range):
-        """Takes a list of particles."""
-        self.ndim = len(search_range)
-        self.search_range = np.atleast_2d(search_range)
-        if not isinstance(points, list):
-            points = list(points)
-        self.points = points
-        self.rebuild()
 
-    def __len__(self):
-        return len(self.points)
 
-    def add_point(self, pt):
-        self.points.append(pt)
-        self._clean = False
+    .. note:: To be used for tracking this class must be sub-classed to provide a :py:func:`distance` function.  Child classes **MUST** call :py:func:`Point.__init__`.  (See :py:class:`~trackpy.tracking.PointND` for example. )
+    '''
+    count = 0
 
-    @property
-    def kdtree(self):
-        if not self._clean:
-            self.rebuild()
-        return self._kdtree
+    def __init__(self):
+        self._track = None
+        self.uuid = Point.count         # unique id for __hash__
+        Point.count += 1
 
-    def rebuild(self, coord_map=None):
-        """Rebuilds tree from ``points`` attribute.
+    ## def __eq__(self, other):
+    ##     return self.uuid == other.uuid
 
-        coord_map : function, optional
+    ## def __neq__(self, other):
+    ##     return not self.__eq__(other)
 
-            Called with a list of N Point instances, returns their
-            "effective" locations, as an N x d array (or list of tuples).
-            Used for prediction (see "predict" module).
-
-        rebuild() needs to be called after ``add_point()`` and
-        before tree is used for spatial queries again (i.e. when
-        memory is turned on).
-        """
-        if coord_map is None:
-            coordmap_as_arr = points_to_arr
-        else:
-            coordmap_as_arr = lambda x: np.asarray(list(coord_map(x)))
-        if len(self.points) == 0:
-            self._kdtree = None
-        else:
-            coords = coordmap_as_arr(self.points) / self.search_range
-            self._kdtree = cKDTree(coords, 15)
-        # This could be tuned
-        self._clean = True
+    def add_to_track(self, track):
+        '''
+        :param track: the track to assign to this :py:class:`Point`
 
-    @property
-    def coords_rescaled(self):
-        if self._clean:
-            if self._kdtree is None:
-                return np.empty((0, self.ndim))
-            else:
-                return self._kdtree.data
-        else:
-            return points_to_arr(self.points) / self.search_range
+        Sets the track of a :py:class:`Point` object.  Raises
+        :py:exc:`Exception` if the object is already assigned a track.
 
 
-class HashTable:
-    """Basic hash table for fast look up of particles in neighborhood.
 
-    Parameters
-    ----------
-    dims : ND tuple
-        the range of the data to be put in the hash table.
-        0<data[k]<dims[k]
-
-    box_size : float
-        how big each box should be in data units.
-        The same scale is used for all dimensions
+        '''
+        if self._track is not None:
+            raise Exception("trying to add a particle already in a track")
+        self._track = track
 
+    def remove_from_track(self, track):
+        '''
+        :param track: the track to disassociate from this :py:class:`Point`
 
-    """
-    class Out_of_hash_excpt(Exception):
-        """
-        :py:exc:`Exception` for indicating that a particle is outside of the
-        valid range for this hash table."""
-        pass
+        Removes this point from the given track. Raises :py:exc:`Exception` if
+        particle not associated with the given track.
 
-    def __init__(self, dims, box_size):
-        '''
-        Sets up the hash table
 
         '''
-        # the dimensions of the data
-        self.dims = dims
-        # the size of boxes to use in the units of the data
-        self.box_size = box_size
-        self.hash_dims = np.ceil(np.array(dims) / box_size)
-
-        self.hash_table = [[] for j in range(int(np.prod(self.hash_dims)))]
-        # how many spatial dimensions
-        self.spat_dims = len(dims)
-        self.cached_shifts = None
-        self.cached_rrange = None
-        self.strides = np.cumprod(
-                           np.concatenate(([1], self.hash_dims[1:])))[::-1]
-        self.points = []
+        if self._track != track:
+            raise Exception("Point not associated with given track")
+        track.remove_point(self)
 
-    def get_region(self, point, rrange):
+    def in_track(self):
         '''
-        Returns all the particles within the region of maximum radius
-        rrange in data units.  This may return Points that are farther
-        than rrange.
-
-        Parameters
-        ----------
-        point : Point
-            point to find the features around
+        :rtype: bool
 
-        rrange: float
-            the size of the ball to search in data units.
+        Returns if a point is associated with a track '''
+        return self._track is not None
 
+    @property
+    def track(self):
+        """Returns the track that this :class:`Point` is in.  May be `None` """
+        return self._track
 
-        '''
-        hash_size = self.hash_dims
-        center = np.floor(point.pos / self.box_size)
-        if any(center >= hash_size) or any(center < 0):
-            raise Hash_table.Out_of_hash_excpt("cord out of range")
 
-        rrange = int(np.ceil(rrange / self.box_size))
+class PointND(Point):
+    '''
+    :param t: a time-like variable.
+    :param pos: position of feature
+    :type pos: iterable of length d
 
-        # check if we have already computed the shifts
-        if rrange == self.cached_rrange and self.cached_shifts is not None:
-            shifts = self.cached_shifts   # if we have, use them
-        # Other wise, generate them
-        else:
-            if self.spat_dims == 2:
-                shifts = [np.array([j, k])
-                          for j in range(-rrange, rrange + 1)
-                          for k in range(-rrange, rrange + 1)]
-            elif self.spat_dims == 3:
-                shifts = [np.array([j, k, m])
-                          for j in range(-rrange, rrange + 1)
-                          for k in range(-rrange, rrange + 1)
-                          for m in range(-rrange, rrange + 1)]
-            else:
-                raise NotImplementedError('only 2 and 3 dimensions implemented')
-            self.cached_rrange = rrange   # and save them
-            self.cached_shifts = shifts
-        region = []
+    Version of :py:class:`Point` for tracking in flat space with
+    non-periodic boundary conditions.
+    '''
 
-        for s in shifts:
+    def __init__(self, t, pos):
+        Point.__init__(self)                  # initialize base class
+        self.t = t                            # time
+        self.pos = np.asarray(pos)            # position in ND space
 
-            cord = center + s
-            if any(cord >= hash_size) or any(cord < 0):
-                continue
-            indx = int(sum(cord * self.strides))
-            region.extend(self.hash_table[indx])
-        return region
+    def distance(self, other_point):
+        '''
+        :param other_point: point to get distance to.
+        :type other_point: :py:class:`~trackpy.tracking.Point`
 
-    def add_point(self, point):
-        """
-        Adds the `point` to the hash table.
+        Returns the absolute distance between this point and other_point
 
-        Assumes that :py:attr:`point.pos` exists and is the array-like.
+        '''
+        return np.sqrt(np.sum((self.pos - other_point.pos) ** 2))
 
-        Parameters
-        ----------
-        point : Point
-            object representing the feature to add to the hash table
+    def __str__(self):
+        return "({t}, {p})".format(t=self.t, p=self.pos)
 
-        """
-        cord = np.floor(np.asarray(point.pos) / self.box_size)
-        hash_size = self.hash_dims
-        if any(cord >= hash_size) or any(cord < 0):
-            raise Hash_table.Out_of_hash_excpt("cord out of range")
-        indx = int(sum(cord * self.strides))
-        self.hash_table[indx].append(point)
-        self.points.append(point)
+    def __repr__(self):
+        coords = '(' + (', '.join(["{:.3f}"]*len(self.pos))).format(*self.pos) + ')'
+        track = " in Track %d" % self.track.indx if self.track else ""
+        return "<%s at %d, " % (self.__class__.__name__, self.t) + coords + track + ">"
 
-    def __len__(self):
-        return len(self.points)
+class IndexedPointND(PointND):
 
-Hash_table = HashTable
+    def __init__(self, t, pos, id):
+        PointND.__init__(self, t, pos)  # initialize base class
+        self.id = id  # unique ID derived from sequential index
 
 
 def link(levels, search_range, hash_generator, memory=0, track_cls=None,
          neighbor_strategy='BTree', link_strategy='recursive'):
     """Link features into trajectories, assigning a label to each trajectory.
 
     This function is deprecated and lacks some recently-added options,
-    though it is still accurate. Use link_df or link_iter.
+    thought it is still accurate. Use link_df or link_iter.
 
     Parameters
     ----------
     levels : iterable of iterables containing Points objects
         e.g., a list containing lists with the Points in each frame
-    search_range : tuple
-        the maximum distance features can move between frames, per dimension
+    search_range : integer
+        the maximum distance features can move between frames
     hash_generator : a function that returns a HashTable
         only used if neighbor_strategy is set to 'BTree' (default)
     memory : integer
         the maximum number of frames during which a feature can vanish,
         then reppear nearby, and be considered the same particle. 0 by default.
     neighbor_strategy : {'BTree', 'KDTree'}
         algorithm used to identify nearby features
-    link_strategy : {'recursive', 'nonrecursive', 'numba', 'drop', 'auto'}
+    link_strategy : {'recursive', 'nonrecursive', 'numba', 'auto'}
         algorithm used to resolve subnetworks of nearby particles
         'auto' uses numba if available
-        'drop' causes particles in subnetworks to go unlinked
 
     Returns
     -------
     tracks : list of Track (or track_cls) objects
 
     See Also
     --------
     link_df, link_iter
     """
     # An informative error to help newbies who go astray
     if isinstance(levels, pd.DataFrame):
         raise TypeError("Instead of link, use link_df, which accepts "
                         "pandas DataFrames.")
+
     if track_cls is None:
         track_cls = Track  # stores Points
     label_generator = link_iter(iter(levels), search_range, memory=memory,
                                 neighbor_strategy=neighbor_strategy,
                                 link_strategy=link_strategy,
                                 track_cls=track_cls,
                                 hash_generator=hash_generator)
@@ -431,184 +389,155 @@
     labels = [label.track.indx for label_list in labels
               for label in label_list]  # flat
     grouped = points.groupby(labels)
     representative_points = grouped.first()  # one point from each Track
     tracks = representative_points.apply(lambda x: x.track)
     return tracks
 
-
 def link_df(features, search_range, memory=0,
             neighbor_strategy='KDTree', link_strategy='auto',
-            predictor=None, adaptive_stop=None, adaptive_step=0.95,
-            copy_features=False, diagnostics=False, pos_columns=None,
-            t_column=None, hash_size=None, box_size=None,
-            verify_integrity=True, retain_index=False):
+            predictor=None, hash_size=None, box_size=None,
+            pos_columns=None, t_column=None, verify_integrity=True,
+            retain_index=False):
     """Link features into trajectories, assigning a label to each trajectory.
 
     Parameters
     ----------
     features : DataFrame
         Must include any number of column(s) for position and a column of
         frame numbers. By default, 'x' and 'y' are expected for position,
         and 'frame' is expected for frame number. See below for options to use
-        custom column names. After linking, this DataFrame will contain a
-        'particle' column.
-    search_range : float
+        custom column names.
+    search_range : integer
         the maximum distance features can move between frames
     memory : integer
         the maximum number of frames during which a feature can vanish,
         then reppear nearby, and be considered the same particle. 0 by default.
     neighbor_strategy : {'KDTree', 'BTree'}
         algorithm used to identify nearby features
-    link_strategy : {'recursive', 'nonrecursive', 'numba', 'drop', 'auto'}
+    link_strategy : {'recursive', 'nonrecursive', 'numba', 'auto'}
         algorithm used to resolve subnetworks of nearby particles
         'auto' uses numba if available
-        'drop' causes particles in subnetworks to go unlinked
-    predictor : function, optional
-        Improve performance by guessing where a particle will be in
-        the next frame.
-
+    predictor : function (optional)
+        Improve performance by guessing where a particle will be in the next frame.
         For examples of how this works, see the "predict" module.
-    adaptive_stop : float, optional
-        If not None, when encountering an oversize subnet, retry by progressively
-        reducing search_range until the subnet is solvable. If search_range
-        becomes <= adaptive_stop, give up and raise a SubnetOversizeException.
-    adaptive_step : float, optional
-        Reduce search_range by multiplying it by this factor.
-    copy_features : boolean
-        Leave the original features DataFrame intact (slower, uses more memory)
-    diagnostics : boolean
-        Collect details about how each particle was linked, and return as
-        columns in the output DataFrame. Implies copy=True.
+
+    Returns
+    -------
+    trajectories : DataFrame
+        This is the input features DataFrame, now with a new column labeling
+        each particle with an ID number. This is not a copy.
+
+    Other Parameters
+    ----------------
     pos_columns : DataFrame column names (unlimited dimensions)
         Default is ['x', 'y']
     t_column : DataFrame column name
         Default is 'frame'
     hash_size : sequence
         For 'BTree' mode only. Define the shape of the search region.
         If None (default), infer shape from range of data.
     box_size : sequence
         For 'BTree' mode only. Define the parition size to optimize
         performance. If None (default), the search_range is used, which is
         a reasonable guess for best performance.
     verify_integrity : boolean
-        False by default for fastest performance.
+        False by default, for fastest performance.
         Use True if you suspect a bug in linking.
     retain_index : boolean
         By default, the index is reset to be sequential. To keep the original
         index, set to True. Default is fine unless you devise a special use.
-
-    Returns
-    -------
-    trajectories : DataFrame
-        This is the input features DataFrame, now with a new column labeling
-        each particle with an ID number. This is not a copy; the original
-        features DataFrame is modified.
     """
     # Assign defaults. (Do it here to avoid "mutable defaults" issue.)
     if pos_columns is None:
         pos_columns = ['x', 'y']
     if t_column is None:
         t_column = 'frame'
-    search_range = validate_tuple(search_range, len(pos_columns))
     if hash_size is None:
-        MARGIN = 1  # avoid OutOfHashException
+        MARGIN = 1 # avoid OutOfHashException
         hash_size = features[pos_columns].max() + MARGIN
 
     # Group the DataFrame by time steps and make a 'level' out of each
     # one, using the index to keep track of Points.
     if retain_index:
         orig_index = features.index.copy()  # Save it; restore it at the end.
     features.reset_index(inplace=True, drop=True)
-    levels = _gen_levels_df(features, pos_columns, t_column, diagnostics)
+    levels = (_build_level(frame, pos_columns, t_column) for frame_no, frame \
+              in features.groupby(t_column))
     labeled_levels = link_iter(
         levels, search_range, memory=memory, predictor=predictor,
-        adaptive_stop=adaptive_stop, adaptive_step=adaptive_step,
         neighbor_strategy=neighbor_strategy, link_strategy=link_strategy,
         hash_size=hash_size, box_size=box_size)
 
-    if diagnostics:
-        features = strip_diagnostics(features)  # Makes a copy
-    elif copy_features:
-        features = features.copy()
-
     # Do the tracking, and update the DataFrame after each iteration.
     features['particle'] = np.nan  # placeholder
     for level in labeled_levels:
-        if len(level) == 0:
-            continue
         index = [x.id for x in level]
         labels = pd.Series([x.track.id for x in level], index)
         frame_no = next(iter(level)).t  # uses an arbitary element from the set
         if verify_integrity:
             # This checks that the labeling is sane and tries
             # to raise informatively if some unknown bug in linking
             # produces a malformed labeling.
             _verify_integrity(frame_no, labels)
             # an additional check particular to link_df
             if len(labels) > len(features[features[t_column] == frame_no]):
                 raise UnknownLinkingError("There are more labels than "
                                           "particles to be labeled in Frame "
-                                          "{}.".format(frame_no))
+                                           "%d".format(frame_no))
         features['particle'].update(labels)
-        if diagnostics:
-            _add_diagnostic_columns(features, level)
 
-        logger.info("Frame %d: %d trajectories present", frame_no, len(labels))
+        msg = "Frame %d: %d trajectories present" % (frame_no, len(labels))
+        print_update(msg)
 
     if retain_index:
         features.index = orig_index
         # And don't bother to sort -- user must be doing something special.
     else:
-        pandas_sort(features, ['particle', t_column], inplace=True)
+        features.sort(['particle', t_column], inplace=True)
         features.reset_index(drop=True, inplace=True)
     return features
 
-
 def link_df_iter(features, search_range, memory=0,
             neighbor_strategy='KDTree', link_strategy='auto',
-            predictor=None, adaptive_stop=None, adaptive_step=0.95,
-            diagnostics=False, pos_columns=None,
-            t_column=None, hash_size=None, box_size=None,
-            verify_integrity=True, retain_index=False):
+            hash_size=None, box_size=None, predictor=None,
+            pos_columns=None, t_column=None, verify_integrity=True,
+            retain_index=False):
     """Link features into trajectories, assigning a label to each trajectory.
 
     Parameters
     ----------
     features : iterable of DataFrames
         Each DataFrame must include any number of column(s) for position and a
-        column of frame numbers. By default, 'x' and 'y' are expected for
-        position, and 'frame' is expected for frame number. See below for
-        options to use custom column names.
-    search_range : float
+        column of frame numbers. By default, 'x' and 'y' are expected for position,
+        and 'frame' is expected for frame number. See below for options to use
+        custom column names.
+    search_range : integer
         the maximum distance features can move between frames
     memory : integer
         the maximum number of frames during which a feature can vanish,
         then reppear nearby, and be considered the same particle. 0 by default.
     neighbor_strategy : {'KDTree', 'BTree'}
         algorithm used to identify nearby features. Note that when using
         BTree, you must specify hash_size
-    link_strategy : {'recursive', 'nonrecursive', 'numba', 'drop', 'auto'}
+    link_strategy : {'recursive', 'nonrecursive', 'numba', 'auto'}
         algorithm used to resolve subnetworks of nearby particles
         'auto' uses numba if available
-        'drop' causes particles in subnetworks to go unlinked
-    predictor : function, optional
-        Improve performance by guessing where a particle will be in the
-        next frame.
-
+    predictor : function (optional)
+        Improve performance by guessing where a particle will be in the next frame.
         For examples of how this works, see the "predict" module.
-    adaptive_stop : float, optional
-        If not None, when encountering an oversize subnet, retry by progressively
-        reducing search_range until the subnet is solvable. If search_range
-        becomes <= adaptive_stop, give up and raise a SubnetOversizeException.
-    adaptive_step : float, optional
-        Reduce search_range by multiplying it by this factor.
-    diagnostics : boolean
-        Collect details about how each particle was linked, and return as
-        columns in the output DataFrame.
+
+    Returns
+    -------
+    trajectories : DataFrame
+        This is the input features DataFrame, now with a new column labeling
+        each particle with an ID number. This is not a copy.
+
+    Other Parameters
+    ----------------
     pos_columns : DataFrame column names (unlimited dimensions)
         Default is ['x', 'y']
     t_column : DataFrame column name
         Default is 'frame'
     hash_size : sequence
         For 'BTree' mode only. Define the shape of the search region.
     box_size : sequence
@@ -617,600 +546,685 @@
         a reasonable guess for best performance.
     verify_integrity : boolean
         False by default, for fastest performance.
         Use True if you suspect a bug in linking.
     retain_index : boolean
         By default, the index is reset to be sequential. To keep the original
         index, set to True. Default is fine unless you devise a special use.
-
-    Returns
-    -------
-    trajectories : DataFrame
-        This is the input features DataFrame, now with a new column labeling
-        each particle with an ID number for each frame.
     """
     # Assign defaults. (Do it here to avoid "mutable defaults" issue.)
     if pos_columns is None:
         pos_columns = ['x', 'y']
     if t_column is None:
         t_column = 'frame'
-    search_range = validate_tuple(search_range, len(pos_columns))
 
     # Group the DataFrame by time steps and make a 'level' out of each
     # one, using the index to keep track of Points.
 
-    # Non-destructively check the type of the first item of features
-    feature_iter, feature_checktype_iter = itertools.tee(iter(features))
-    try:  # If it quacks like a DataFrame...
-        next(feature_checktype_iter).reset_index()
-    except AttributeError:
-        raise ValueError("Features data must be an iterable of DataFrames, one per "
-                         "video frame. Use link_df() if you have a single DataFrame "
-                         "describing multiple frames.")
-    del feature_checktype_iter  # Otherwise pipes will back up.
-
+    feature_iter = iter(features)
     # To allow retain_index
     features_for_reset, features_forindex = itertools.tee(feature_iter)
     index_iter = (fr.index.copy() for fr in features_forindex)
     # To allow extra columns to be recovered later
     features_forlinking, features_forpost = itertools.tee(
-        frame.reset_index(drop=True) for frame in features_for_reset)
-    # make a generator over the frames
-    levels = (_build_level(frame, pos_columns, t_column, diagnostics=diagnostics)
-                         for frame in features_forlinking)
-
-    # make a generator of the levels post-linking
+        (frame.reset_index(drop=True) for frame in features_for_reset))
+    levels = (_build_level(frame, pos_columns, t_column) \
+                                                for frame in features_forlinking)
     labeled_levels = link_iter(
         levels, search_range, memory=memory, predictor=predictor,
-        adaptive_stop=adaptive_stop, adaptive_step=adaptive_step,
         neighbor_strategy=neighbor_strategy, link_strategy=link_strategy,
         hash_size=hash_size, box_size=box_size)
 
     # Re-assemble the features data, now with track labels and (if desired)
     # the original index.
     for labeled_level, source_features, old_index in zip(
             labeled_levels, features_forpost, index_iter):
         features = source_features.copy()
         features['particle'] = np.nan  # placeholder
-        index = [x.id for x in labeled_level]
+        index = [x.id for x in  labeled_level]
         labels = pd.Series([x.track.id for x in labeled_level], index)
-        # uses an arbitary element from the set
-        frame_no = next(iter(labeled_level)).t
+        frame_no = next(iter(labeled_level)).t  # uses an arbitary element from the set
         if verify_integrity:
             # This checks that the labeling is sane and tries
             # to raise informatively if some unknown bug in linking
             # produces a malformed labeling.
             _verify_integrity(frame_no, labels)
             # additional checks particular to link_df_iter
-            if not all(frame_no == source_features[t_column].values):
-                raise UnknownLinkingError(("The features passed for Frame {} "
+            if not all(frame_no == source_features.frame.values):
+                raise UnknownLinkingError("The features passed for Frame %d "
                                           "do not all share the same frame "
-                                          "number.").format(frame_no))
+                                          "number.".format(frame_no))
             if len(labels) > len(features):
                 raise UnknownLinkingError("There are more labels than "
                                           "particles to be labeled in Frame "
-                                           "{}.".format(frame_no))
+                                           "%d".format(frame_no))
         features['particle'].update(labels)
-        if diagnostics:
-            _add_diagnostic_columns(features, labeled_level)
 
         if retain_index:
             features.index = old_index
-            # TODO: don't run index.copy() even when retain_index is false
         else:
-            pandas_sort(features, 'particle', inplace=True)
+            features.sort('particle', inplace=True)
             features.reset_index(drop=True, inplace=True)
 
-        logger.info("Frame %d: %d trajectories present", frame_no, len(labels))
+        msg = "Frame %d: %d trajectories present" % (frame_no, len(labels))
+        print_update(msg)
 
         yield features
 
+def _build_level(frame, pos_columns, t_column):
+    "Return IndexPointND objects for a DataFrame of points."
+    build_pt = lambda x: IndexedPointND(x[1], x[0][1].values, x[0][0])
+    # iterrows() returns: (index which we use as feature id, data)
+    zipped = zip(frame[pos_columns].iterrows(), frame[t_column])
+    return [build_pt(pt) for pt in zipped]
 
-def _build_level(frame, pos_columns, t_column, diagnostics=False):
-    """Return PointND objects for a DataFrame of points.
-
-    Parameters
-    ----------
-    frame : DataFrame
-        Unlinked points data.
-    pos_columns : list
-        Names of position columns in "frame"
-    t_column : string
-        Name of time column in "frame"
-    diagnostics : boolean, optional
-        Whether resulting point objects should collect diagnostic information.
-    """
-    if diagnostics:
-        point_cls = PointNDDiagnostics
-    else:
-        point_cls = PointND
-    # This is the only chance to do this, as only here the point_cls is known.
-    if not hasattr(point_cls, 'counter'):
-        point_cls.reset_counter()
-    return list(map(point_cls, frame[t_column],
-                    frame[pos_columns].values, frame.index))
-
-
-def _gen_levels_df(df, pos_columns, t_column, diagnostics=False):
-    """Return a generator of PointND objects for a DataFrame of points.
-
-    The DataFrame is assumed to contain integer framenumbers. For a missing
-    frame number, an empty list is returned.
-
-    Parameters
-    ----------
-    df : DataFrame
-        Unlinked points data for all frames.
-    pos_columns : list
-        Names of position columns in "frame"
-    t_column : string
-        Name of time column in "frame"
-    diagnostics : boolean, optional
-        Whether resulting point objects should collect diagnostic information.
-    """
-    grouped = iter(df.groupby(t_column))
-    cur_frame, frame = next(grouped)
-    cur_frame += 1.5  # set counter to 1.5 for issues with e.g. 1.000001
-    yield _build_level(frame, pos_columns, t_column, diagnostics)
-
-    for frame_no, frame in grouped:
-        while cur_frame < frame_no:
-            cur_frame += 1
-            yield []
-
-        cur_frame += 1
-        yield _build_level(frame, pos_columns, t_column, diagnostics)
-
-
-def _add_diagnostic_columns(features, level):
-    """Copy the diagnostic information stored in each particle to the
-    corresponding columns in 'features'. Create columns as needed."""
-    diag = pd.DataFrame({x.id: x.diag for x in level}, dtype=object).T
-    diag.columns = ['diag_' + cn for cn in diag.columns]
-    for cn in diag.columns:
-        if cn not in features.columns:
-            features[cn] = pd.Series(np.nan, dtype=float, index=features.index)
-    features.update(diag)
-
-
-def strip_diagnostics(tracks):
-    """Remove diagnostic information from a tracks DataFrame.
-
-    This returns a copy of the DataFrame. Columns with names that start
-    with "diag_" are excluded."""
-    base_cols = [cn for cn in tracks.columns if not cn.startswith('diag_')]
-    return tracks.reindex(columns=base_cols)
+class UnknownLinkingError(Exception):
+    pass
 
 
 def _verify_integrity(frame_no, labels):
     if labels.duplicated().sum() > 0:
         raise UnknownLinkingError(
-            "There are two particles with the same label in Frame {}.".format(
+            "There are two particles with the same label in Frame %d.".format(
                 frame_no))
     if np.any(labels < 0):
         raise UnknownLinkingError("Some particles were not labeled "
-                                  "in Frame {}.".format(frame_no))
-
+                                  "in Frame %d.".format(frame_no))
 
 def link_iter(levels, search_range, memory=0,
               neighbor_strategy='KDTree', link_strategy='auto',
               hash_size=None, box_size=None, predictor=None,
-              adaptive_stop=None, adaptive_step=0.95,
               track_cls=None, hash_generator=None):
     """Link features into trajectories, assigning a label to each trajectory.
 
-    This function is a generator which yields at each step the Point
-    objects for the current level.  These objects know what trajectory
-    they are in.
-
     Parameters
     ----------
     levels : iterable of iterables containing Points objects
         e.g., a list containing lists with the Points in each frame
-    search_range : tuple
-        the maximum distance features can move between frames, per dimension
+    search_range : integer
+        the maximum distance features can move between frames
     memory : integer
         the maximum number of frames during which a feature can vanish,
         then reppear nearby, and be considered the same particle. 0 by default.
     neighbor_strategy : {'KDTree', 'BTree'}
         algorithm used to identify nearby features
-    link_strategy : {'recursive', 'nonrecursive', 'numba', 'drop', 'auto'}
+    link_strategy : {'recursive', 'nonrecursive', 'numba', 'auto'}
         algorithm used to resolve subnetworks of nearby particles
         'auto' uses numba if available
-        'drop' causes particles in subnetworks to go unlinked
+    predictor : function (optional)
+        Improve performance by guessing where a particle will be in the next frame.
+        For examples of how this works, see the "predict" module.
+
+    Yields
+    ------
+    labels : list of integers
+       labeling the features in the given level
+
+    Other Parameters
+    ----------------
     hash_size : sequence
         For 'BTree' mode only. Define the shape of the search region.
         (Higher-level wrappers of link infer this from the data.)
     box_size : sequence
         For 'BTree' mode only. Define the parition size to optimize
         performance. If None (default), the search_range is used, which is
         a reasonable guess for best performance.
-    predictor : function, optional
-        Improve performance by guessing where a particle will be in the
-        next frame.
-        For examples of how this works, see the "predict" module.
-    adaptive_stop : float, optional
-        If not None, when encountering an oversize subnet, retry by progressively
-        reducing search_range until the subnet is solvable. If search_range
-        becomes <= adaptive_stop, give up and raise a SubnetOversizeException.
-    adaptive_step : float, optional
-        Reduce search_range by multiplying it by this factor.
-    track_cls : class, optional
+    track_cls : class (optional)
         for special uses, you can specify a custom class that holds
         each Track
-    hash_generator : function, optional
+    hash_generator : function (optional)
         a function that returns a HashTable, included for legacy support.
         Specifying hash_size and box_size (above) fully defined a HashTable.
-
-    Returns
-    -------
-    cur_level : iterable of Point objects
-        The labeled points at each level.
     """
-    if not hasattr(search_range, '__iter__'):
-        # We need to know the dimensionality of the image, but this information
-        # is not accessible at this point. Guess 2D and give a warning.
-        search_range = (search_range,) * 2
-        warn("In link and link_iter, search_range should be given as a "
-             "tuple with the same length as the number of dimensions in "
-             "the image. We now assume the dimensionality to be 2D.")
-    linker = Linker(search_range, memory=memory, neighbor_strategy=neighbor_strategy,
-                 link_strategy=link_strategy, hash_size=hash_size,
-                 box_size=box_size, predictor=predictor,
-                 adaptive_stop=adaptive_stop, adaptive_step=adaptive_step,
-                 track_cls=track_cls, hash_generator=hash_generator)
-    return linker.link(levels)
-
-class Linker:
-    """See link_iter() for a description of parameters."""
-    # Largest subnet we will attempt to solve.
-    MAX_SUB_NET_SIZE = 30
-    # For adaptive search, subnet linking should fail much faster.
-    MAX_SUB_NET_SIZE_ADAPTIVE = 15
-
-    def __init__(self, search_range, memory=0,
-              neighbor_strategy='KDTree', link_strategy='auto',
-              hash_size=None, box_size=None, predictor=None,
-              adaptive_stop=None, adaptive_step=0.95,
-              track_cls=None, hash_generator=None):
-        self.search_range = search_range
-        self.memory = memory
-        self.predictor = predictor
-        self.adaptive_stop = adaptive_stop
-        self.adaptive_step = adaptive_step
-        if track_cls is None:
-            track_cls = TrackUnstored  # does not store Points
-        track_cls.reset_counter()
-        self.track_cls = track_cls
-        self.hash_generator = hash_generator
-        self.neighbor_strategy = neighbor_strategy
-
-        self.diag = False  # Whether to save diagnostic info
-
-        if self.hash_generator is None:
-            if neighbor_strategy == 'BTree':
-                if hash_size is None:
-                    raise ValueError("In 'BTree' mode, you must specify hash_size")
-                if box_size is None:
-                    box_size = search_range[0]
-            self.hash_generator = lambda: Hash_table(hash_size, box_size)
-
-        linkers = {'recursive': recursive_linker_obj,
-                   'nonrecursive': nonrecursive_link,
-                   'drop': drop_link}
-        if NUMBA_AVAILABLE:
-            linkers['numba'] = numba_link
-            linkers['auto'] = linkers['numba']
-        else:
-            linkers['auto'] = linkers['recursive']
-        try:
-            self.subnet_linker = linkers[link_strategy]
-        except KeyError:
-            raise ValueError("link_strategy must be one of: " + ', '.join(linkers.keys()))
-
-        if self.neighbor_strategy not in ['KDTree', 'BTree']:
-            raise ValueError("neighbor_strategy must be 'KDTree' or 'BTree'")
-        if self.neighbor_strategy == 'BTree' and not is_isotropic(self.search_range):
-            raise ValueError("The neighbor_strategy 'BTree' cannot deal with "
-                             "anisotropic search ranges. Please use 'KDTree'.")
-
-        if self.adaptive_stop is not None:
-            # adaptive_stop is a fraction of search range
-            self.adaptive_stop = self.adaptive_stop / np.min(self.search_range)
-            if 1 * self.adaptive_stop <= 0:
-                raise ValueError("adaptive_stop must be positive.")
-            self.max_subnet_size = self.MAX_SUB_NET_SIZE_ADAPTIVE
-        else:
-            self.max_subnet_size = self.MAX_SUB_NET_SIZE
+    if hash_generator is None:
+        if neighbor_strategy == 'BTree':
+            if hash_size is None:
+                raise ValueError("In 'BTree' mode, you must specify hash_size")
+            if box_size is None:
+                box_size = search_range
+        hash_generator = lambda: Hash_table(hash_size, box_size)
+    if track_cls is None:
+        track_cls = DummyTrack  # does not store Points
 
-        if 1 * self.adaptive_step <= 0 or 1 * self.adaptive_step >= 1:
-            raise ValueError("adaptive_step must be between "
-                             "0 and 1 non-inclusive.")
-
-        self.subnet_counter = 0  # Unique ID for each subnet
-
-    def link(self, levels):
-        level_iter = iter(levels)
-        prev_level = next(level_iter)
-        prev_set = set(prev_level)
-
-        # Only save diagnostic info if it's possible. This saves
-        # 1-2% execution time and significant memory.
-        # We just check the first particle in the first level.
-        self.diag = hasattr(next(iter(prev_level)), 'diag')
-
-        # Make a Hash / Tree for the first level.
-        if self.neighbor_strategy == 'BTree':
-            prev_hash = self.hash_generator()
-            for p in prev_set:
-                prev_hash.add_point(p)
-        elif self.neighbor_strategy == 'KDTree':
-            prev_hash = TreeFinder(prev_level, self.search_range)
+    linkers = {'recursive': recursive_linker_obj,
+               'nonrecursive': nonrecursive_link}
+    if NUMBA_AVAILABLE:
+        linkers['numba'] = numba_link
+        linkers['auto'] = linkers['numba']
+    else:
+        linkers['auto'] = linkers['recursive']
+    try:
+        subnet_linker = linkers[link_strategy]
+    except KeyError:
+        raise ValueError("link_strategy must be one of: " + ', '.join(linkers.keys()))
+
+    if neighbor_strategy not in ['KDTree', 'BTree']:
+        raise ValueError("neighbor_strategy must be 'KDTree' or 'BTree'")
+
+    level_iter = iter(levels)
+    prev_level = next(level_iter)
+    prev_set = set(prev_level)
 
+    # Make a Hash / Tree for the first level.
+    if neighbor_strategy == 'BTree':
+        prev_hash = hash_generator()
         for p in prev_set:
-            p.forward_cands = []
+            prev_hash.add_point(p)
+    elif neighbor_strategy == 'KDTree':
+        prev_hash = TreeFinder(prev_level)
 
-        try:
-            # Start ID numbers from zero, incompatible with multithreading.
-            self.track_cls.reset_counter()
-        except AttributeError:
-            # must be using a custom Track class without this method
-            pass
-
-        # Assume everything in first level starts a Track.
-        # Iterate over prev_level, not prev_set, because order -> track ID.
-        for p in prev_level:
-            self.track_cls(p)
-        self.mem_set = set()
-
-        # Initialize memory with empty sets.
-        mem_history = []
-        for j in range(self.memory):
-            mem_history.append(set())
-
-        yield list(prev_set)  # Short-circuit the loop on first call.
-
-        for cur_level in levels:
-            # Create the set for the destination level.
-            cur_set = set(cur_level)
-            tmp_set = set(cur_level)  # copy used in next loop iteration
-
-            # First, a bit of unfinished business:
-            # If prediction is enabled, we need to update the positions in prev_hash
-            # to where we think they'll be in the frame corresponding to cur_level.
-            if self.predictor is not None:
-                # This only works for KDTree right now, because KDTree can store particle
-                # positions in a separate data structure from the PointND instances.
-                if not isinstance(prev_hash, TreeFinder):
-                    raise NotImplementedError(
-                        'Prediction works with the "KDTree" neighbor_strategy only.')
-                # Get the time of cur_level from its first particle
-                t_next = list(itertools.islice(cur_level, 0, 1))[0].t
-                targeted_predictor = functools.partial(self.predictor, t_next)
-                prev_hash.rebuild(coord_map=targeted_predictor) # Rewrite positions
-
-            # Now we can process the new particles.
-            # Make a Hash / Tree for the destination level.
-            if self.neighbor_strategy == 'BTree':
-                cur_hash = self.hash_generator()
-                for p in cur_set:
-                    cur_hash.add_point(p)
-            elif self.neighbor_strategy == 'KDTree':
-                cur_hash = TreeFinder(cur_level, self.search_range)
+    for p in prev_set:
+        p.forward_cands = []
 
-            # Set up attributes for keeping track of possible connections.
-            for p in cur_set:
-                p.back_cands = []
-                p.forward_cands = []
+    try:
+        # Start ID numbers from zero, incompatible with multithreading.
+        track_cls.reset_counter()
+    except AttributeError:
+        # must be using a custom Track class without this method
+        pass
 
-            # Sort out what can go to what. This uses the search_range to
-            # rescale distances between particles in between 0 and 1. From here
-            # on, search_range = 1.
-            assign_candidates(cur_hash, prev_hash, self.search_range,
-                              self.neighbor_strategy)
 
-            # sort the candidate lists by distance
+    # Assume everything in first level starts a Track.
+    track_lst = [track_cls(p) for p in prev_set]
+    mem_set = set()
+
+    # Initialize memory with empty sets.
+    mem_history = []
+    for j in range(memory):
+        mem_history.append(set())
+
+    yield list(prev_set)  # Short-circuit the loop on first call.
+
+    for cur_level in levels:
+        # Create the set for the destination level.
+        cur_set = set(cur_level)
+        tmp_set = set(cur_level)  # copy used in next loop iteration
+
+        # First, a bit of unfinished business:
+        # If prediction is enabled, we need to update the positions in prev_hash
+        # to where we think they'll be in the frame corresponding to cur_level.
+        if predictor is not None:
+            # This only works for KDTree right now, because KDTree can store particle
+            # positions in a separate data structure from the PointND instances.
+            if not isinstance(prev_hash, TreeFinder):
+                raise NotImplementedError(
+                    'Prediction works with the "KDTree" neighbor_strategy only.')
+            # Get the time of cur_level from its first particle
+            t_next = list(itertools.islice(cur_level, 0, 1))[0].t
+            targeted_predictor = functools.partial(predictor, t_next)
+            prev_hash.rebuild(coord_map=targeted_predictor) # Rewrite positions
+
+        # Now we can process the new particles.
+        # Make a Hash / Tree for the destination level.
+        if neighbor_strategy == 'BTree':
+            cur_hash = hash_generator()
             for p in cur_set:
-                p.back_cands.sort(key=lambda x: x[1])
-            for p in prev_set:
-                p.forward_cands.sort(key=lambda x: x[1])
-
-            # Note that this modifies cur_set, prev_set, but that's OK.
-            spl, dpl = self._assign_links(cur_set, prev_set, search_range=1.)
-
-            new_mem_set = set()
-            for sp, dp in zip(spl, dpl):
-                # Do linking
-                if sp is not None and dp is not None:
-                    sp.track.add_point(dp)
-                    if sp in self.mem_set:  # Very rare
-                        self.mem_set.remove(sp)
-                elif sp is None:
-                    # if unclaimed destination particle, a track is born!
-                    self.track_cls(dp)
-                elif dp is None:
-                    # add the unmatched source particles to the new
-                    # memory set
-                    new_mem_set.add(sp)
-
-                # Clean up
-                if dp is not None:
-                    del dp.back_cands
-                if sp is not None:
-                    del sp.forward_cands
-
-            # TODO: Emit debug message with number of
-            # subnets in this level, numbers of new/remembered/lost particles
-
-            # yield the current level before we add the memory points to it
-            yield cur_level
+                cur_hash.add_point(p)
+        elif neighbor_strategy == 'KDTree':
+            cur_hash = TreeFinder(cur_level)
+
+        # Set up attributes for keeping track of possible connections.
+        for p in cur_set:
+            p.back_cands = []
+            p.forward_cands = []
 
-            # set prev_hash to cur hash
-            prev_hash = cur_hash
+        # Sort out what can go to what.
+        assign_candidates(cur_level, prev_hash, search_range,
+                          neighbor_strategy)
+
+        # sort the candidate lists by distance
+        for p in cur_set:
+            p.back_cands.sort(key=lambda x: x[1])
+        for p in prev_set:
+            p.forward_cands.sort(key=lambda x: x[1])
 
-            # add in the memory points
-            # store the current level for use in next loop
-            if self.memory > 0:
-                # identify the new memory points
-                new_mem_set -= self.mem_set
-                mem_history.append(new_mem_set)
-                # remove points that are now too old
-                self.mem_set -= mem_history.pop(0)
-                # add the new points
-                self.mem_set |= new_mem_set
-                # add the memory particles to what will be the next source set
-                tmp_set |= self.mem_set
-                # add memory points to prev_hash (to be used as the next source)
-                for m in self.mem_set:
-                    # add points to the hash
-                    prev_hash.add_point(m)
-                    # Record how many times this particle got "held back".
-                    # Since this particle has already been yielded in a previous
-                    # level, we can't store it there. We'll have to put it in the
-                    # track object, then copy this info to the point in cur_hash
-                    # if/when we make a link.
-                    m.track.incr_memory()
-                    # re-create the forward_cands list
-                    m.forward_cands = []
-
-            prev_set = tmp_set
-
-    def _assign_links(self, dest_set, source_set, search_range):
-        """Match particles in dest_set with source_set.
-
-        Returns source, dest lists of equal length, corresponding
-        to pairs of source and destination particles. A 'None' value
-        denotes that a match was not found.
-
-        The contents of dest_set and source_set will be changed, as
-        well as the forward_cands and back_cands attributes of the
-        particles. However, this does not meaningfully change the state
-        within link(). All meaningful actions are taken within link(),
-        based on the recommendations of _assign_links().
-        """
-        spl, dpl = [], []
-        diag = self.diag
-        # while there are particles left to link, link
-        while len(dest_set) > 0:
-            p = dest_set.pop()
+        new_mem_set = set()
+        # while there are particles left to link, linkge the repo
+        while len(cur_set) > 0:
+            p = cur_set.pop()
             bc_c = len(p.back_cands)
             # no backwards candidates
             if bc_c == 0:
-                # particle will get a new track
-                dpl.append(p)
-                spl.append(None)
-                if diag:
-                    p.diag['search_range'] = search_range
-                continue  # do next dest_set particle
+                # add a new track
+                track_lst.append(track_cls(p))
+                # clean up tracking apparatus
+                del p.back_cands
+                # short circuit loop
+                continue
             if bc_c == 1:
                 # one backwards candidate
                 b_c_p = p.back_cands[0]
-                # and only one forward candidate
+                # and only one forward candidatege the repo
                 b_c_p_0 = b_c_p[0]
                 if len(b_c_p_0.forward_cands) == 1:
-                    # schedule these particles for linking
-                    dpl.append(p)
-                    spl.append(b_c_p_0)
-                    source_set.discard(b_c_p_0)
-                    if diag:
-                        p.diag['search_range'] = search_range
-                    continue  # do next dest_set particle
+                    # add to the track of the candidate
+                    b_c_p_0.track.add_point(p)
+                    _maybe_remove(mem_set, b_c_p_0)
+                    # clean up tracking apparatus
+                    del p.back_cands
+                    del b_c_p_0.forward_cands
+                    prev_set.discard(b_c_p_0)
+                    # short circuit loop
+                    continue
             # we need to generate the sub networks
             done_flg = False
             s_sn = set()                  # source sub net
             d_sn = set()                  # destination sub net
             # add working particle to destination sub-net
             d_sn.add(p)
             while not done_flg:
                 d_sn_sz = len(d_sn)
                 s_sn_sz = len(s_sn)
                 for dp in d_sn:
                     for c_sp in dp.back_cands:
                         s_sn.add(c_sp[0])
-                        source_set.discard(c_sp[0])
+                        prev_set.discard(c_sp[0])
                 for sp in s_sn:
                     for c_dp in sp.forward_cands:
                         d_sn.add(c_dp[0])
-                        dest_set.discard(c_dp[0])
+                        cur_set.discard(c_dp[0])
                 done_flg = (len(d_sn) == d_sn_sz) and (len(s_sn) == s_sn_sz)
 
-            # sort and add in penalty for not linking
+            # add in penalty for not linking
             for _s in s_sn:
-                # If we end up having to recurse for adaptive search, this final
-                # element will be dropped and re-added, because search_range is
-                # decreasing.
-                _s.forward_cands.sort(key=lambda x: x[1])
                 _s.forward_cands.append((None, search_range))
 
-            try:
-                sn_spl, sn_dpl = self.subnet_linker(s_sn, len(d_sn), search_range,
-                                                    max_size=self.max_subnet_size,
-                                                    diag=diag)
-
-                if diag:
-                    # Record information about this invocation of the subnet linker.
-                    for dp in d_sn:
-                        dp.diag['subnet'] = self.subnet_counter
-                        dp.diag['subnet_size'] = len(s_sn)
-                        dp.diag['search_range'] = search_range
-                for dp in d_sn - set(sn_dpl):
-                    # Unclaimed destination particle in subnet
-                    sn_spl.append(None)
-                    sn_dpl.append(dp)
-                self.subnet_counter += 1
-            except SubnetOversizeException:
-                if self.adaptive_stop is None:
-                    raise
-                # Reduce search_range
-                new_range = search_range * self.adaptive_step
-                if search_range <= self.adaptive_stop:
-                    # adaptive_stop is the search_range below which linking
-                    # is presumed invalid. So we just give up.
-                    raise
+            spl, dpl = subnet_linker(s_sn, len(d_sn), search_range)
 
-                # Prune the candidate lists of s_sn, d_sn; then recurse.
-                for sp in s_sn:
-                    sp.forward_cands = [fc for fc in sp.forward_cands
-                                        if fc[1] <= new_range]
-                for dp in d_sn:
-                    dp.back_cands = [bc for bc in dp.back_cands
-                                     if bc[1] <= new_range]
-                sn_spl, sn_dpl = self._assign_links(
-                    d_sn, s_sn, new_range)
+            # Identify the particles in the destination set that
+            # were not linked to.
+            d_remain = set(d for d in d_sn if d is not None)  # TODO DAN
+            d_remain -= set(d for d in dpl if d is not None)
+            for dp in d_remain:
+                # if unclaimed destination particle, a track is born!
+                track_lst.append(track_cls(dp))
+                # clean up
+                del dp.back_cands
 
-            spl.extend(sn_spl)
-            dpl.extend(sn_dpl)
+            for sp, dp in zip(spl, dpl):
+                # do linking and clean up
+                if sp is not None and dp is not None:
+                    sp.track.add_point(dp)
+                    _maybe_remove(mem_set, sp)
+                if dp is not None:  # TODO DAN 'Should never happen' - Nathan
+                    del dp.back_cands
+                if sp is not None:
+                    del sp.forward_cands
+                    if dp is None:
+                        # add the unmatched source particles to the new
+                        # memory set
+                        new_mem_set.add(sp)
+
+        # Remember the source particles left unlinked that were not in
+        # a subnetwork.
+        for sp in prev_set:
+            new_mem_set.add(sp)
+
+        # set prev_hash to cur hash
+        prev_hash = cur_hash
+
+        # add in the memory points
+        # store the current level for use in next loop
+        if memory > 0:
+            # identify the new memory points
+            new_mem_set -= mem_set
+            mem_history.append(new_mem_set)
+            # remove points that are now too old
+            mem_set -= mem_history.pop(0)
+            # add the new points
+            mem_set |= new_mem_set
+            # add the memory particles to what will be the next source
+            # set
+            tmp_set |= mem_set
+            # add memory points to prev_hash (to be used as the next source)
+            for m in mem_set:
+                # add points to the hash
+                prev_hash.add_point(m)
+                # re-create the forward_cands list
+                m.forward_cands = []
 
-        # Leftovers
-        for pp in source_set:
-            spl.append(pp)
-            dpl.append(None)
+        prev_set = tmp_set
 
-        return spl, dpl
+        yield cur_level
 
 
-def assign_candidates(cur_hash, prev_hash, search_range, neighbor_strategy):
+def assign_candidates(cur_level, prev_hash, search_range, neighbor_strategy):
     if neighbor_strategy == 'BTree':
-        if not is_isotropic(search_range):
-            raise ValueError
-        search_range_1d = search_range[0]
         # (Tom's code)
-        for p in cur_hash.points:
-            work_box = prev_hash.get_region(p, search_range_1d)
+        for p in cur_level:
+            # get
+            work_box = prev_hash.get_region(p, search_range)
             for wp in work_box:
-                d = p.distance(wp) / search_range_1d
-                if d < 1.:
+                # this should get changed to deal with squared values
+                # to save an eventually square root
+                d = p.distance(wp)
+                if d < search_range:
                     p.back_cands.append((wp, d))
                     wp.forward_cands.append((p, d))
     elif neighbor_strategy == 'KDTree':
-        # kdtree.query() would raise exception on empty level.
-        if len(cur_hash) and len(prev_hash):
-            cur_coords = cur_hash.coords_rescaled
-            hashpts = prev_hash.points
-            dists, inds = prev_hash.kdtree.query(cur_coords, 10,
-                                                 distance_upper_bound=1+1e-7)
-            nn = np.sum(np.isfinite(dists), 1)  # Number of neighbors of each particle
-            for i, p in enumerate(cur_hash.points):
-                for j in range(nn[i]):
-                    wp = hashpts[inds[i, j]]
-                    p.back_cands.append((wp, dists[i, j]))
-                    wp.forward_cands.append((p, dists[i, j]))
+        hashpts = prev_hash.points
+        cur_coords = np.array([x.pos for x in cur_level])
+        dists, inds = prev_hash.kdtree.query(cur_coords, 10, distance_upper_bound=search_range)
+        nn = np.sum(np.isfinite(dists), 1) # Number of neighbors of each particle
+        for i, p in enumerate(cur_level):
+            for j in range(nn[i]):
+                wp = hashpts[inds[i,j]]
+                p.back_cands.append((wp, dists[i,j]))
+                wp.forward_cands.append((p, dists[i,j]))
+
+
+class SubnetOversizeException(Exception):
+    '''An :py:exc:`Exception` to be raised when the sub-nets are too
+    big to be efficiently linked.  If you get this then either reduce your search range
+    or increase :py:attr:`sub_net_linker.MAX_SUB_NET_SIZE`'''
+    pass
+
+
+def recursive_linker_obj(s_sn, dest_size, search_range):
+    snl = sub_net_linker(s_sn, dest_size, search_range)
+    return zip(*snl.best_pairs)
+
+
+class SubnetLinker(object):
+    '''A helper class for implementing the Crocker-Grier tracking
+    algorithm.  This class handles the recursion code for the sub-net linking'''
+    MAX_SUB_NET_SIZE = 50
+
+    def __init__(self, s_sn, dest_size, search_range):
+        #        print 'made sub linker'
+        self.s_sn = s_sn
+        self.search_range = search_range
+        self.s_lst = [s for s in s_sn]
+        self.s_lst.sort(key=lambda x: len(x.forward_cands))
+        self.MAX = len(self.s_lst)
+
+        self.max_links = min(self.MAX, dest_size)
+        self.best_pairs = None
+        self.cur_pairs = deque([])
+        self.best_sum = np.Inf
+        self.d_taken = set()
+        self.cur_sum = 0
+
+        if self.MAX > sub_net_linker.MAX_SUB_NET_SIZE:
+            raise SubnetOversizeException("Subnetwork contains %d points"
+                                          % self.MAX)
+        # do the computation
+        self.do_recur(0)
+
+    def do_recur(self, j):
+        cur_s = self.s_lst[j]
+        for cur_d, dist in cur_s.forward_cands:
+            tmp_sum = self.cur_sum + dist
+            if tmp_sum > self.best_sum:
+                # if we are already greater than the best sum, bail we
+                # can bail all the way out of this branch because all
+                # the other possible connections (including the null
+                # connection) are more expensive than the current
+                # connection, thus we can discard with out testing all
+                # leaves down this branch
+                return
+            if cur_d is not None and cur_d in self.d_taken:
+                # we have already used this destination point, bail
+                continue
+            # add this pair to the running list
+            self.cur_pairs.append((cur_s, cur_d))
+            # add the destination point to the exclusion list
+            if cur_d is not None:
+                self.d_taken.add(cur_d)
+            # update the current sum
+            self.cur_sum = tmp_sum
+            # buried base case
+            # if we have hit the end of s_lst and made it this far, it
+            # must be a better linking so save it.
+            if j + 1 == self.MAX:
+                tmp_sum = self.cur_sum + self.search_range * (self.max_links - len(self.d_taken))
+                if tmp_sum < self.best_sum:
+                    self.best_sum = tmp_sum
+                    self.best_pairs = list(self.cur_pairs)
+            else:
+                # re curse!
+                self.do_recur(j + 1)
+            # remove this step from the working
+            self.cur_sum -= dist
+            if cur_d is not None:
+                self.d_taken.remove(cur_d)
+            self.cur_pairs.pop()
+        pass
+
+
+def nonrecursive_link(source_list, dest_size, search_range):
+
+    #    print 'non-recursive', len(source_list), dest_size
+    source_list = list(source_list)
+    source_list.sort(key=lambda x: len(x.forward_cands))
+    MAX = len(source_list)
+
+    max_links = min(MAX, dest_size)
+    k_stack = deque([0])
+    j = 0
+    cur_back = deque([])
+    cur_sum_stack = deque([0])
+
+    best_sum = np.inf
+
+    best_back = None
+    cand_list_list = [c.forward_cands for c in source_list]
+    cand_lens = [len(c) for c in cand_list_list]
+
+    while j >= 0:
+        # grab everything from the end of the stack
+        cur_sum = cur_sum_stack[-1]
+        if j >= MAX:
+            # base case, no more source candidates,
+            # save the current configuration if it's better than the current max
+            # add penalty for not linking to particles in the destination set
+            tmp_sum = cur_sum + search_range * (max_links - len([d for d in cur_back if d is not None]))
+            if tmp_sum < best_sum:
+                best_sum = cur_sum
+                best_back = list(cur_back)
+
+            j -= 1
+            k_stack.pop()
+            cur_sum_stack.pop()
+            cur_back.pop()
+
+            # print 'we have a winner'
+            # print '-------------------------'
+            continue
+
+        # see if we have any forward candidates
+        k = k_stack[-1]
+        if k >= cand_lens[j]:
+            # no more candidates to try, this branch is done
+            j -= 1
+            k_stack.pop()
+            cur_sum_stack.pop()
+            if j >= 0:
+                cur_back.pop()
+            # print 'out of cands'
+            # print '-------------------------'
+            continue
+
+        # get the forward candidate
+        cur_d, cur_dist = cand_list_list[j][k]
+
+        tmp_sum = cur_sum + cur_dist
+        if tmp_sum > best_sum:
+            # nothing in this branch can do better than the current best
+            j -= 1
+            k_stack.pop()
+            cur_sum_stack.pop()
+            if j >= 0:
+                cur_back.pop()
+            # print 'total bail'
+            # print '-------------------------'
+            continue
+
+        # advance the counter in the k_stack, the next time this level
+        # of the frame stack is run the _next_ candidate will be run
+        k_stack[-1] += 1
+        # check if it's already linked
+        if cur_d is not None and cur_d in cur_back:
+            # this will run the loop with almost identical stack, but with advanced k
+            # print 'already linked cur_d'
+            # print '-------------------------'
+            continue
+
+        j += 1
+        k_stack.append(0)
+        cur_sum_stack.append(tmp_sum)
+        cur_back.append(cur_d)
+
+        # print '-------------------------'
+    #    print 'done'
+    return source_list, best_back
+
+def numba_link(s_sn, dest_size, search_radius):
+    """Recursively find the optimal bonds for a group of particles between 2 frames.
+
+    This is only invoked when there is more than one possibility within
+    ``search_radius``.
+
+    Note that ``dest_size`` is unused; it is determined from the contents of
+    the source list.
+    """
+    # The basic idea: replace Point objects with integer indices into lists of Points.
+    # Then the hard part (recursion) runs quickly because it is just passing arrays.
+    # In fact, we can compile it with numba so that it runs in acceptable time.
+    max_candidates = 9 # Max forward candidates we expect for any particle
+    src_net = list(s_sn)
+    nj = len(src_net) # j will index the source particles
+    if nj > SubnetLinker.MAX_SUB_NET_SIZE:
+        raise SubnetOversizeException('search_range (aka maxdisp) too large for reasonable performance on these data (sub net contains %d points)' % nj)
+    # Build arrays of all destination (forward) candidates and their distances
+    dcands = set()
+    for p in src_net:
+        dcands.update([cand for cand, dist in p.forward_cands])
+    dcands = list(dcands)
+    dcands_map = {cand: i for i, cand in enumerate(dcands)}
+    # A source particle's actual candidates only take up the start of
+    # each row of the array. All other elements represent the null link option
+    # (i.e. particle lost)
+    candsarray = np.ones((nj, max_candidates + 1), dtype=np.int64) * -1
+    distsarray = np.ones((nj, max_candidates + 1), dtype=np.float64) * search_radius
+    ncands = np.zeros((nj,), dtype=np.int64)
+    for j, sp in enumerate(src_net):
+        ncands[j] = len(sp.forward_cands)
+        if ncands[j] > max_candidates:
+            raise SubnetOversizeException('search_range (aka maxdisp) too large for reasonable performance on these data (particle has %i forward candidates)' % ncands[j])
+        candsarray[j,:ncands[j]] = [dcands_map[cand] for cand, dist in sp.forward_cands]
+        distsarray[j,:ncands[j]] = [dist for cand, dist in sp.forward_cands]
+    # The assignments are persistent across levels of the recursion
+    best_assignments = np.ones((nj,), dtype=np.int64) * -1
+    cur_assignments = np.ones((nj,), dtype=np.int64) * -1
+    tmp_assignments = np.zeros((nj,), dtype=np.int64)
+    cur_sums = np.zeros((nj,), dtype=np.float64)
+    # In the next line, distsarray is passed in quadrature so that adding distances works.
+    bestsum = _numba_subnet_norecur(ncands, candsarray, distsarray**2, cur_assignments, cur_sums,
+            tmp_assignments, best_assignments)
+    if bestsum < 0:
+        raise SubnetOversizeException('search_range (aka maxdisp) too large for reasonable performance on these data (exceeded max iterations for subnet)')
+    # Return particle objects. Account for every source particle we were given.
+    # 'None' denotes a null link and will be used for the memory feature.
+    return zip(*[(src_net[j], (dcands[i] if i >= 0 else None)) \
+            for j, i in enumerate(best_assignments)])
+
+@try_numba_autojit
+def _numba_subnet_norecur(ncands, candsarray, dists2array, cur_assignments, cur_sums, tmp_assignments, best_assignments):
+    """Find the optimal track assigments for a subnetwork, without recursion.
+
+    This is for nj source particles. All arguments are arrays with nj rows.
+
+    cur_assignments, tmp_assignments are just temporary registers of length nj.
+    best_assignments is modified in place.
+    Returns the best sum.
+    """
+    itercount = 0
+    nj = candsarray.shape[0]
+    tmp_sum = 0.
+    best_sum = 1.0e23
+    j = 0
+    while 1:
+        itercount += 1
+        if itercount >= 500000000:
+            return -1.0
+        delta = 0 # What to do at the end
+        # This is an endless loop. We go up and down levels of recursion,
+        # and emulate the mechanics of nested "for" loops, using the
+        # blocks of code marked "GO UP" and "GO DOWN". It's not pretty.
+
+        # Load state from the "stack"
+        i = tmp_assignments[j]
+        #if j == 0:
+        #    print i, j, best_sum
+        #    sys.stdout.flush()
+        if i > ncands[j]:
+            # We've exhausted possibilities at this level, including the
+            # null link; make no more changes and go up a level
+            #### GO UP
+            delta = -1
+        else:
+            tmp_sum = cur_sums[j] + dists2array[j,i]
+            if tmp_sum > best_sum:
+                # if we are already greater than the best sum, bail. we
+                # can bail all the way out of this branch because all
+                # the other possible connections (including the null
+                # connection) are more expensive than the current
+                # connection, thus we can discard with out testing all
+                # leaves down this branch
+                #### GO UP
+                delta = -1
+            else:
+                # We have to seriously consider this candidate.
+                # We can have as many null links as we want, but the real particles are finite
+                # This loop looks inefficient but it's what numba wants!
+                flag = 0
+                for jtmp in range(nj):
+                    if cur_assignments[jtmp] == candsarray[j,i]:
+                        if jtmp < j:
+                            flag = 1
+                if flag and candsarray[j,i] >= 0:
+                    # we have already used this destination point; try the next one instead
+                    delta = 0
+                else:
+                    cur_assignments[j] = candsarray[j,i]
+                    # OK, I guess we'll try this assignment
+                    if j + 1 == nj:
+                        # We have made assignments for all the particles,
+                        # and we never exceeded the previous best_sum.
+                        # This is our new optimum.
+                        #print 'hit: %f' % best_sum
+                        best_sum = tmp_sum
+                        # This array is shared by all levels of recursion.
+                        # If it's not touched again, it will be used once we
+                        # get back to link_subnet
+                        for tmpj in range(nj):
+                            best_assignments[tmpj] = cur_assignments[tmpj]
+                        #### GO UP
+                        delta = -1
+                    else:
+                        # Try various assignments for the next particle
+                        #### GO DOWN
+                        delta = 1
+        if delta == -1:
+            if j > 0:
+                j += -1
+                tmp_assignments[j] += 1 # Try the next candidate at this higher level
+                continue
+            else:
+                return best_sum
+        elif delta == 1:
+            j += 1
+            cur_sums[j] = tmp_sum # Floor for all subsequent sums
+            tmp_assignments[j] = 0
+        else:
+            tmp_assignments[j] += 1
+
+def _maybe_remove(s, p):
+    # Begging forgiveness is faster than asking permission
+    try:
+        s.remove(p)
+    except KeyError:
+        pass
+
+sub_net_linker = SubnetLinker  # legacy
+Hash_table = HashTable  # legacy
```

### Comparing `trackpy-0.6.3rc1/trackpy/motion.py` & `trackpy-unknown/trackpy/motion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
+
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
-
-import warnings
-from warnings import warn
-from .utils import pandas_sort, pandas_concat, guess_pos_columns
+from scipy import interpolate
+from scipy.spatial import cKDTree
 
 
-def msd(traj, mpp, fps, max_lagtime=100, detail=False, pos_columns=None):
+def msd(traj, mpp, fps, max_lagtime=100, detail=False):
     """Compute the mean displacement and mean squared displacement of one
     trajectory over a range of time intervals.
 
     Parameters
     ----------
     traj : DataFrame with one trajectory, including columns frame, x, and y
     mpp : microns per pixel
@@ -20,156 +22,46 @@
         Default: 100
     detail : See below. Default False.
 
     Returns
     -------
     DataFrame([<x>, <y>, <x^2>, <y^2>, msd], index=t)
 
-        If detail is True, the DataFrame also contains a column N,
-        the estimated number of statistically independent measurements
-        that comprise the result at each lagtime.
+    If detail is True, the DataFrame also contains a column N,
+    the estimated number of statistically independent measurements
+    that comprise the result at each lagtime.
 
     Notes
     -----
     Input units are pixels and frames. Output units are microns and seconds.
 
     See also
     --------
-    imsd
-    emsd
-    """
-    if traj['frame'].max() - traj['frame'].min() + 1 == len(traj):
-        # no gaps: use fourier-transform algorithm
-        return _msd_fft(traj, mpp, fps, max_lagtime, detail, pos_columns)
-    else:
-        # there are gaps in the trajectory: use slower algorithm
-        return _msd_gaps(traj, mpp, fps, max_lagtime, detail, pos_columns)
-
-
-def _msd_N(N, t):
-    """Computes the effective number of statistically independent measurements
-    of the mean square displacement of a single trajectory.
-
-    Parameters
-    ----------
-    N : integer
-        the number of positions in the trajectory (=number of steps + 1)
-    t : iterable
-        an iterable of lagtimes (integers)
-
-    References
-    ----------
-    Derived from Equation B4 in:
-    Qian, Hong, Michael P. Sheetz, and Elliot L. Elson. "Single particle
-    tracking. Analysis of diffusion and flow in two-dimensional systems."
-    Biophysical journal 60.4 (1991): 910.
+    imsd() and emsd()
     """
-    t = np.array(t, dtype=float)
-    return np.where(t > N/2,
-                    1/(1+((N-t)**3+5*t-4*(N-t)**2*t-N)/(6*(N-t)*t**2)),
-                    6*(N-t)**2*t/(2*N-t+4*N*t**2-5*t**3))
-
-
-def _msd_iter(pos, lagtimes):
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=RuntimeWarning)
-        for lt in lagtimes:
-            diff = pos[lt:] - pos[:-lt]
-            yield np.concatenate((np.nanmean(diff, axis=0),
-                                  np.nanmean(diff**2, axis=0)))
-
-
-
-def _msd_gaps(traj, mpp, fps, max_lagtime=100, detail=False, pos_columns=None):
-    """Compute the mean displacement and mean squared displacement of one
-    trajectory over a range of time intervals."""
-    if pos_columns is None:
-        pos_columns = ['x', 'y']
-    result_columns = ['<{}>'.format(p) for p in pos_columns] + \
-                     ['<{}^2>'.format(p) for p in pos_columns]
-
-    # The following fails if > 1 record per particle (cannot reindex):
-    try:
-        # Reindex with consecutive frames, placing NaNs in the gaps.
-        pos = traj.set_index('frame')[pos_columns] * mpp
-        pos = pos.reindex(np.arange(pos.index[0], 1 + pos.index[-1]))
-    except ValueError:
-        if traj['frame'].nunique()!=len(traj['frame']):
-            # Reindex failed due to duplicate index values
-            raise Exception("Cannot use msd_gaps, more than one trajectory "
-                            "per particle found.")
-        else:
-            raise
-
-
-
-    max_lagtime = min(max_lagtime, len(pos) - 1)  # checking to be safe
-
-    lagtimes = np.arange(1, max_lagtime + 1)
-
-    result = pd.DataFrame(_msd_iter(pos.values, lagtimes),
-                          columns=result_columns, index=lagtimes)
-    result['msd'] = result[result_columns[-len(pos_columns):]].sum(1)
-    if detail:
-        # effective number of measurements
-        # approximately corrected with number of gaps
-        result['N'] = _msd_N(len(pos), lagtimes) * len(traj) / len(pos)
-    result['lagt'] = result.index.values/float(fps)
-    result.index.name = 'lagt'
-    return result
-
-
-def _msd_fft(traj, mpp, fps, max_lagtime=100, detail=False, pos_columns=None):
-    """Compute the mean displacement and mean squared displacement of one
-    trajectory over a range of time intervals using FFT transformation.
-
-    The original Python implementation comes from a SO answer :
-    http://stackoverflow.com/questions/34222272/computing-mean-square-displacement-using-python-and-fft#34222273.
-    The algorithm is described in this paper : http://dx.doi.org/10.1051/sfn/201112010.
-    """
-    if pos_columns is None:
-        pos_columns = ['x', 'y']
-    result_columns = ['<{}>'.format(p) for p in pos_columns] + \
-                     ['<{}^2>'.format(p) for p in pos_columns]
-
-    r = traj[pos_columns].values * mpp
+    pos = traj.set_index('frame')[['x', 'y']]
     t = traj['frame']
-
-    max_lagtime = min(max_lagtime, len(t) - 1)  # checking to be safe
-    lagtimes = np.arange(1, max_lagtime + 1)
-    N = len(r)
-
-    # calculate the mean displacements
-    r_diff = r[:-max_lagtime-1:-1] - r[:max_lagtime]
-    disp = np.cumsum(r_diff, axis=0) / (N - lagtimes[:, np.newaxis])
-
-    # below is a vectorized version of the original code
-    D = r**2
-    D_sum = D[:max_lagtime] + D[:-max_lagtime-1:-1]
-    S1 = 2*D.sum(axis=0) - np.cumsum(D_sum, axis=0)
-    F = np.fft.fft(r, n=2*N, axis=0)  # 2*N because of zero-padding
-    PSD = F * F.conjugate()
-    # this is the autocorrelation in convention B:
-    S2 = np.fft.ifft(PSD, axis=0)[1:max_lagtime+1].real
-    squared_disp = S1 - 2 * S2
-    squared_disp /= N - lagtimes[:, np.newaxis]  # divide res(m) by (N-m)
-
-    results = pd.DataFrame(np.concatenate((disp, squared_disp), axis=1),
-                           index=lagtimes, columns=result_columns)
-    results['msd'] = squared_disp.sum(axis=1)
+    # Reindex with consecutive frames, placing NaNs in the gaps.
+    pos = pos.reindex(np.arange(pos.index[0], 1 + pos.index[-1]))
+    max_lagtime = min(max_lagtime, len(t)) # checking to be safe
+    lagtimes = 1 + np.arange(max_lagtime)
+    disp = pd.concat([pos.sub(pos.shift(lt)) for lt in lagtimes],
+                     keys=lagtimes, names=['lagt', 'frames'])
+    results = mpp*disp.mean(level=0)
+    results.columns = ['<x>', '<y>']
+    results[['<x^2>', '<y^2>']] = mpp**2*(disp**2).mean(level=0)
+    results['msd'] = mpp**2*(disp**2).mean(level=0).sum(1) # <r^2>
+    # Estimated statistically independent measurements = 2N/t
     if detail:
-        results['N'] = _msd_N(N, lagtimes)
-    results['lagt'] = lagtimes / float(fps)
-    results.index.name = 'lagt'
-
-    return results
+        results['N'] = 2*disp.icol(0).count(level=0).div(Series(lagtimes))
+    results['lagt'] = results.index.values/fps
+    return results[:-1]
 
-
-def imsd(traj, mpp, fps, max_lagtime=100, statistic='msd', pos_columns=None):
-    """Compute the mean squared displacement of each particle.
+def imsd(traj, mpp, fps, max_lagtime=100, statistic='msd'):
+    """Compute the mean squared displacements of particles individually.
 
     Parameters
     ----------
     traj : DataFrame of trajectories of multiple particles, including
         columns particle, frame, x, and y
     mpp : microns per pixel
     fps : frames per second
@@ -188,27 +80,26 @@
     Input units are pixels and frames. Output units are microns and seconds.
     """
     ids = []
     msds = []
     # Note: Index is set by msd, so we don't need to worry
     # about conformity here.
     for pid, ptraj in traj.groupby('particle'):
-        msds.append(msd(ptraj, mpp, fps, max_lagtime, False, pos_columns))
+        msds.append(msd(ptraj, mpp, fps, max_lagtime, False))
         ids.append(pid)
-    results = pandas_concat(msds, keys=ids)
+    results = pd.concat(msds, keys=ids)
     # Swap MultiIndex levels so that unstack() makes particles into columns.
     results = results.swaplevel(0, 1)[statistic].unstack()
     lagt = results.index.values.astype('float64')/float(fps)
     results.set_index(lagt, inplace=True)
     results.index.name = 'lag time [s]'
     return results
 
-
-def emsd(traj, mpp, fps, max_lagtime=100, detail=False, pos_columns=None):
-    """Compute the ensemble mean squared displacements of many particles.
+def emsd(traj, mpp, fps, max_lagtime=100, detail=False):
+    """Compute the mean squared displacements of an ensemble of particles.
 
     Parameters
     ----------
     traj : DataFrame of trajectories of multiple particles, including
         columns particle, frame, x, and y
     mpp : microns per pixel
     fps : frames per second
@@ -225,319 +116,254 @@
     Notes
     -----
     Input units are pixels and frames. Output units are microns and seconds.
     """
     ids = []
     msds = []
     for pid, ptraj in traj.reset_index(drop=True).groupby('particle'):
-        msds.append(msd(ptraj, mpp, fps, max_lagtime, True, pos_columns))
+        msds.append(msd(ptraj, mpp, fps, max_lagtime, True))
         ids.append(pid)
-    msds = pandas_concat(msds, keys=ids, names=['particle', 'frame'])
-    results = msds.mul(msds['N'], axis=0).groupby(level=1).mean()  # weighted average
-    results = results.div(msds['N'].groupby(level=1).mean(), axis=0)  # weights normalized
+    msds = pd.concat(msds, keys=ids, names=['particle', 'frame'])
+    results = msds.mul(msds['N'], axis=0).mean(level=1) # weighted average
+    results = results.div(msds['N'].mean(level=1), axis=0) # weights normalized
     # Above, lagt is lumped in with the rest for simplicity and speed.
     # Here, rebuild it from the frame index.
     if not detail:
         return results.set_index('lagt')['msd']
-    # correctly compute the effective number of independent measurements
-    results['N'] = msds['N'].groupby(level=1).sum()
     return results
 
-
-def compute_drift(traj, smoothing=0, pos_columns=None):
-    """Return the ensemble drift, xy(t).
+def compute_drift(traj, smoothing=0):
+    """Return the ensemble drift, x(t).
 
     Parameters
     ----------
-    traj : DataFrame
-        trajectories, including position columns, 'frame', and 'particle'
-    smoothing : integer, optional
+    traj : DataFrame of trajectories, including columns x, y, frame, and particle
+    smoothing : integer
         Smooth the drift using a forward-looking rolling mean over
-        this many frames. Default: 0.
-    pos_columns : list, optional
-        The names of the position columns.
-        Default ['y', 'x'] or ['z', 'y', 'x'] if 'z' is present in traj.
+        this many frames.
 
     Returns
     -------
-    drift : DataFrame(pos_columns, index=frame)
+    drift : DataFrame([x, y], index=frame)
 
     Examples
     --------
-    >>> compute_drift(traj).plot()
-    >>> compute_drift(traj, 0, ['x', 'y']).plot() # not smoothed, equivalent to default.
-    >>> compute_drift(traj, 15).plot() # Try various smoothing values.
-    >>> drift = compute_drift(traj, 15) # Save good drift curves.
-    >>> corrected_traj = subtract_drift(traj, drift) # Apply them.
-    """
-    if pos_columns is None:
-        # swap the order for backwards compatibility
-        pos_columns = guess_pos_columns(traj)
-    f_sort = pandas_sort(traj, ['particle', 'frame'])
-
-    # Compute the difference list of positions, particle, and frame columns.
-    f_diff = f_sort[list(pos_columns) + ['particle', 'frame']].diff()
-
-    # Rename the frame column and insert the original frame column back in.
-    f_diff.rename(columns={'frame': 'frame_diff'}, inplace=True)
-    f_diff['frame'] = f_sort['frame']
-
-    # Compute the per frame averages. Keep only deltas of the same particle,
-    # and between frames that are consecutive.
-    mask = (f_diff['particle'] == 0) & (f_diff['frame_diff'] == 1)
-    dx = f_diff.loc[mask, list(pos_columns) + ['frame']].groupby('frame').mean()
+    compute_drift(traj).plot() # Default smoothing usually smooths too much.
+    compute_drift(traj, 0).plot() # not smoothed
+    compute_drift(traj, 15).plot() # Try various smoothing values.
+
+    drift = compute_drift(traj, 15) # Save good drift curves.
+    corrected_traj = subtract_drift(traj, drift) # Apply them.
+    """
+    # Probe by particle, take the difference between frames.
+    delta = pd.concat([t.set_index('frame', drop=False).diff()
+                       for p, t in traj.groupby('particle')])
+    # Keep only deltas between frames that are consecutive.
+    delta = delta[delta['frame'] == 1]
+    # Restore the original frame column (replacing delta frame).
+    del delta['frame']
+    delta.reset_index(inplace=True)
+    dx = delta.groupby('frame').mean()
     if smoothing > 0:
-        dx = dx.rolling(smoothing, min_periods=0).mean()
-    return dx.cumsum()
+        dx = pd.rolling_mean(dx, smoothing, min_periods=0)
+    x = dx.cumsum(0)[['x', 'y']]
+    return x
 
-
-def subtract_drift(traj, drift=None, inplace=False):
-    """Return a copy of particle trajectories with the overall drift subtracted
-    out.
+def subtract_drift(traj, drift=None):
+    """Return a copy of particle trajectores with the overall drift subtracted out.
 
     Parameters
     ----------
-    traj : DataFrame of trajectories, including columns x, y, frame,
-           and particle (if there is more than one particle).
+    traj : DataFrame of trajectories, including columns x, y, and frame
     drift : optional DataFrame([x, y], index=frame) like output of
          compute_drift(). If no drift is passed, drift is computed from traj.
 
     Returns
     -------
     traj : a copy, having modified columns x and y
     """
+
     if drift is None:
         drift = compute_drift(traj)
-    if not inplace:
-        traj = traj.copy()
-    if 'particle' in traj.columns:
-        traj.set_index(['frame', 'particle'], inplace=True, drop=False)
-    else:
-        traj.set_index(['frame'], inplace=True, drop=False)
-    # Order of particles is irrelevant for performance
-    traj.sort_index(level='frame', inplace=True)
-    for col in drift.columns:
-        traj[col] = traj[col].sub(drift[col], fill_value=0, level='frame')
-    return traj
-
+    return traj.set_index('frame', drop=False).sub(drift, fill_value=0)
 
-def is_typical(msds, frame, lower=0.1, upper=0.9):
-    """Identify which paritcles' MSDs are in the central quantile.
+def is_typical(msds, frame=23, lower=0.1, upper=0.9):
+    """Examine individual particle MSDs, distinguishing outliers from those
+    in the central quantile.
 
     Parameters
     ----------
-    msds : DataFrame
-        This should be organized like the output of imsd().
-        Columns correspond to particles, indexed by lagtime in frames.
-    frame : integer
-        Compare MSDs at this lag interval.
+    msds : DataFrame like the output of imsd()
+        Columns correspond to particles, indexed by lagtime measured in frames.
+    frame : integer frame number
+        Compare MSDs at this lagtime. Default is 23 (1 second at 24 fps).
     lower : float between 0 and 1, default 0.1
         Probes with MSD up to this quantile are deemed outliers.
     upper : float between 0 and 1, default 0.9
         Probes with MSD above this quantile are deemed outliers.
 
+
     Returns
     -------
     Series of boolean values, indexed by particle number
     True = typical particle, False = outlier particle
 
-    Examples
-    --------
-
-    >>> m = tp.imsd(traj, MPP, FPS)
-    >>> # Index by particle ID, slice using boolean output from is_typical(), and then
-    >>> # restore the original index, frame number.
-    >>> typical_traj = traj.set_index('particle').ix[is_typical(m)]\
-    .reset_index().set_index('frame', drop=False)
+    Example
+    -------
+    m = tp.imsd(traj, MPP, FPS)
+    # Index by particle ID, slice using boolean output from is_typical(), and then
+    # restore the original index, frame number.
+    typical_traj = traj.set_index('particle').ix[is_typical(m)].reset_index()\
+        .set_index('frame', drop=False)
     """
     a, b = msds.iloc[frame].quantile(lower), msds.iloc[frame].quantile(upper)
     return (msds.iloc[frame] > a) & (msds.iloc[frame] < b)
 
-
-def vanhove(pos, lagtime, mpp=1, ensemble=False, bins=24):
-    """Compute the van Hove correlation (histogram of displacements).
-
-    The van Hove correlation function is simply a histogram of particle
-    displacements. It is useful for detecting physical heterogeneity
-    (or tracking errors).
+def vanhove(pos, lagtime=23, mpp=1, ensemble=False, bins=24):
+    """Compute the van Hove correlation function at given lagtime (frame span).
 
     Parameters
     ----------
-    pos : DataFrame
-        x or (or!) y positions, one column per particle, indexed by frame
+    pos : DataFrame of x or (or!) y positions, one column per particle, indexed
+        by frame
     lagtime : integer interval of frames
-        Compare the correlation function at this lagtime.
+        Compare the correlation function at this lagtime. Default is 23
+        (1 second at 24 fps).
     mpp : microns per pixel, DEFAULT TO 1 because it is usually fine to use
         pixels for this analysis
     ensemble : boolean, defaults False
     bins : integer or sequence
         Specify a number of equally spaced bins, or explicitly specifiy a
         sequence of bin edges. See np.histogram docs.
 
     Returns
     -------
-    vh : DataFrame or Series
-        If ensemble=True, a DataFrame with each particle's van Hove correlation
+    vh : If ensemble=True, a DataFrame with each particle's van Hove correlation
         function, indexed by displacement. If ensemble=False, a Series with
         the van Hove correlation function of the whole ensemble.
 
-    Examples
-    --------
-    >>> pos = traj.set_index(['frame', 'particle'])['x'].unstack() # particles as columns
-    >>> vh = vanhove(pos)
+    Example
+    -------
+    pos = traj.set_index(['frame', 'particle'])['x'].unstack() # particles as columns
+    vh = vanhove(pos)
     """
     # Reindex with consecutive frames, placing NaNs in the gaps.
     pos = pos.reindex(np.arange(pos.index[0], 1 + pos.index[-1]))
     assert lagtime <= pos.index.values.max(), \
-        "There is a no data out to frame %s. " % pos.index.values.max()
+        "There is a no data out to frame %s. " % frame
     disp = mpp*pos.sub(pos.shift(lagtime))
     # Let np.histogram choose the best bins for all the data together.
     values = disp.values.flatten()
     values = values[np.isfinite(values)]
     global_bins = np.histogram(values, bins=bins)[1]
     # Use those bins to histogram each column by itself.
     vh = disp.apply(
         lambda x: Series(np.histogram(x, bins=global_bins, density=True)[0]))
     vh.index = global_bins[:-1]
     if ensemble:
         return vh.sum(1)/len(vh.columns)
     else:
         return vh
 
-
-def diagonal_size(single_trajectory, pos_columns=None, t_column='frame'):
+def diagonal_size(single_trajectory, pos_columns=['x', 'y'], t_column='frame'):
     """Measure the diagonal size of a trajectory.
 
     Parameters
     ----------
     single_trajectory : DataFrame containing a single trajectory
-    pos_columns = list
-        names of column with position ['x', 'y']
+    pos_columns = ['x', 'y']
     t_column = 'frame'
 
     Returns
     -------
     float : length of diangonal of rectangular box containing the trajectory
 
-    Examples
-    --------
+    Example
+    -------
     >>> diagonal_size(single_trajectory)
 
     >>> many_trajectories.groupby('particle').agg(tp.diagonal_size)
 
     >>> many_trajectories.groupby('particle').filter(lambda x: tp.diagonal_size(x) > 5)
     """
-    if pos_columns is None:
-        pos_columns = ['x', 'y']
+
     pos = single_trajectory.set_index(t_column)[pos_columns]
     return np.sqrt(np.sum(pos.apply(np.ptp)**2))
 
-
 def is_localized(traj, threshold=0.4):
     raise NotImplementedError("This function has been removed.")
 
-
 def is_diffusive(traj, threshold=0.9):
     raise NotImplementedError("This function has been removed.")
 
-
-def relate_frames(t, frame1, frame2, pos_columns=None):
-    """Find the displacement vector of all particles between two frames.
-
-    Parameters
-    ----------
-    t : DataFrame
-        trajectories
-    pos_columns = list
-        names of column with position ['x', 'y']
-    frame1 : integer
-    frame2 : integer
-
-    Returns
-    -------
-    DataFrame
-        indexed by particle, containing:
-        x, y, etc. (corresponding to frame1)
-        x_b, y_b, etc. (corresponding to frame2)
-        dx, dy, etc.
-        dr
-        direction (only if pos_columns=['x', 'y'])
-    """
-    if pos_columns is None:
-        pos_columns = ['x', 'y']
+def relate_frames(t, frame1, frame2):
     a = t[t.frame == frame1]
     b = t[t.frame == frame2]
-    j = a.set_index('particle')[pos_columns].join(
-         b.set_index('particle')[pos_columns], rsuffix='_b')
-    for pos in pos_columns:
-        j['d' + pos] = j[pos + '_b'] - j[pos]
-    j['dr'] = np.sqrt(np.sum([j['d' + pos]**2 for pos in pos_columns], 0))
-    if pos_columns == ['x', 'y']:
-        j['direction'] = np.arctan2(j.dy, j.dx)
+    j = a.set_index('particle')[['x', 'y']].join(
+         b.set_index('particle')[['x', 'y']], rsuffix='_b')
+    j['dx'] = j.x_b - j.x
+    j['dy'] = j.y_b - j.y
+    j['dr'] = np.sqrt(j['dx']**2 + j['dy']**2)
+    j['direction']  = np.arctan2(j.dy, j.dx)
     return j
 
-
 def direction_corr(t, frame1, frame2):
     """Compute the cosine between every pair of particles' displacements.
 
     Parameters
     ----------
-    t : DataFrame
-        trajectories, containing columns particle, frame, x, and y
+    t : DataFrame containing columns particle, frame, x, and y
     frame1 : frame number
     frame2 : frame number
 
     Returns
     -------
-    DataFrame for all particle pairs, including dx, dy, and direction
+    DataFrame, indexed by particle, including dx, dy, and direction
     """
     j = relate_frames(t, frame1, frame2)
-    cosine = np.cos(np.subtract.outer(j.direction.values, j.direction.values))
-    r = np.sqrt(np.subtract.outer(j.x.values, j.x.values)**2 +
-                np.subtract.outer(j.y.values, j.y.values)**2)
+    cosine = np.cos(np.subtract.outer(j.direction, j.direction))
+    r = np.sqrt(np.subtract.outer(j.x, j.x)**2 +
+                np.subtract.outer(j.y, j.y)**2)
     upper_triangle = np.triu_indices_from(r, 1)
     result = DataFrame({'r': r[upper_triangle],
                         'cos': cosine[upper_triangle]})
     return result
 
-
 def velocity_corr(t, frame1, frame2):
     """Compute the velocity correlation between
     every pair of particles' displacements.
 
     Parameters
     ----------
-    t : DataFrame
-        trajectories, containing columns particle, frame, x, and y
+    t : DataFrame containing columns particle, frame, x, and y
     frame1 : frame number
     frame2 : frame number
 
     Returns
     -------
     DataFrame, indexed by particle, including dx, dy, and direction
     """
     j = relate_frames(t, frame1, frame2)
-    cosine = np.cos(np.subtract.outer(j.direction.values, j.direction.values))
-    r = np.sqrt(np.subtract.outer(j.x.values, j.x.values)**2 +
-                np.subtract.outer(j.y.values, j.y.values)**2)
-    dot_product = cosine*np.abs(np.multiply.outer(j.dr.values, j.dr.values))
+    cosine = np.cos(np.subtract.outer(j.direction, j.direction))
+    r = np.sqrt(np.subtract.outer(j.x, j.x)**2 +
+                np.subtract.outer(j.y, j.y)**2)
+    dot_product = cosine*np.abs(np.multiply.outer(j.dr, j.dr))
     upper_triangle = np.triu_indices_from(r, 1)
     result = DataFrame({'r': r[upper_triangle],
                         'dot_product': dot_product[upper_triangle]})
     return result
 
-
 def theta_entropy(pos, bins=24, plot=True):
-    """Plot the distribution of directions and return its Shannon entropy.
+    """Plot the distrbution of directions and return its Shannon entropy.
 
     Parameters
     ----------
     pos : DataFrame with columns x and y, indexed by frame
     bins : number of equally-spaced bins in distribution. Default 24.
-    plot : plot direction histogram if True
+    plot : plot direction historgram if True
 
     Returns
     -------
     float : Shannon entropy
 
     Examples
     --------
@@ -549,24 +375,21 @@
     disp = pos - pos.shift(1)
     direction = np.arctan2(disp['y'], disp['x'])
     bins = np.linspace(-np.pi, np.pi, bins + 1)
     if plot:
         Series(direction).hist(bins=bins)
     return shannon_entropy(direction.dropna(), bins)
 
-
 def shannon_entropy(x, bins):
     """Compute the Shannon entropy of the distribution of x."""
     hist = np.histogram(x, bins)[0]
     hist = hist.astype('float64')/hist.sum()  # normalize probablity dist.
-    with np.errstate(all='ignore'):
-        entropy = -np.sum(np.nan_to_num(hist*np.log(hist)))
+    entropy = -np.sum(np.nan_to_num(hist*np.log(hist)))
     return entropy
 
-
 def min_rolling_theta_entropy(pos, window=24, bins=24):
     """Compute the minimum Shannon entropy in any window.
 
     Parameters
     ----------
     pos : DataFrame with columns x and y, indexed by frame
     window : number of observations per window
@@ -586,19 +409,41 @@
 
     disp = pos - pos.shift(1)
     direction = np.arctan2(disp['y'], disp['x'])
     bins = np.linspace(-np.pi, np.pi, bins + 1)
     f = lambda x: shannon_entropy(x, bins)
     return pd.rolling_apply(direction.dropna(), window, f).min()
 
+def proximity(features, pos_columns=['x', 'y']):
+    """Find the distance to each feature's nearest neighbor.
 
-def proximity(*args, **kwargs):
-    """
-    Deprecated
+    Parameters
+    ----------
+    features : DataFrame
+    pos_columns : list of column names
+        ['x', 'y'] by default
 
-    See also
-    --------
-    trackpy.static.proximity
+    Returns
+    -------
+    proximity : DataFrame
+        distance to each particle's nearest neighbor,
+        indexed by particle if 'particle' column is present in input
+
+    Example
+    -------
+    Find the proximity of each particle to its nearest neighbor in every frame.
+
+    >>> prox = t.groupby('frame').apply(proximity).reset_index()
+    >>> avg_prox = prox.groupby('particle')['proximity'].mean()
+
+    And filter the trajectories...
+
+    >>> particle_nos = avg_prox[avg_prox > 20].index
+    >>> t_filtered = t[t['particle'].isin(particle_nos)]
     """
-    warn('This function has been moved to `trackpy.static', DeprecationWarning)
-    from trackpy.static import proximity
-    return proximity(*args, **kwargs)
+    leaf_size = max(1, int(np.round(np.log10(len(features)))))
+    tree = cKDTree(features[['x', 'y']].copy(), leaf_size)
+    proximity = tree.query(tree.data, 2)[0][:, 1]
+    result = DataFrame({'proximity': proximity})
+    if 'particle' in features:
+        result.set_index(features['particle'], inplace=True)
+    return result
```

### Comparing `trackpy-0.6.3rc1/trackpy/predict.py` & `trackpy-unknown/trackpy/predict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,60 @@
 # Copyright 2014, Nathan C. Keim
 # keimnathan@gmail.com
 
 """Tools to improve tracking performance by guessing where a particle will appear next."""
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
+from six.moves import zip
+
+from copy import copy
 from warnings import warn
 from collections import deque
 import functools, itertools
 
 import numpy as np
 from scipy.interpolate import NearestNDInterpolator, interp1d
 import pandas as pd
 
 from . import linking
 
-from .utils import pandas_concat, guess_pos_columns
-
-
 def predictor(predict_func):
     """Decorator to vectorize a predictor function for a single particle.
 
     Converts P(t1, particle) into Pvec(t1, particles), where 'particles' is a list
     of particle instances, and 'Pvec' can be passed to a linking function
     (e.g. link_df_iter()) via its 'predictor' argument.
     """
     def Pvec(t1, particles):
         targeted_p = functools.partial(predict_func, t1)
         return map(targeted_p, particles)
     return Pvec
 
-
 @predictor
 def null_predict(t1, particle):
     return (particle.pos)
 
-
-class NullPredict:
+class NullPredict(object):
     """Predict that particles will not move.
 
     (Equivalent to standard behavior of linker.)
     """
-    def wrap(self, linking_fcn, *args, **kw):
-        """Wrapper for an arbitrary linking function that causes it to use this predictor.
-
-        The linking function must accept a 'predictor' keyword argument.
-
-        The linking function must accept a 'predictor' keyword argument. It
-        must return an iterator of DataFrames, emitting a DataFrame each time
-        a frame is linked.
-        """
+    def link_df_iter(self, *args, **kw):
+        """Wrapper for linking.link_df_iter() that causes it to use this predictor."""
         if getattr(self, '_already_linked', False):
             warn('Perform tracking with a fresh predictor instance to avoid surprises.')
         self._already_linked = True
         kw['predictor'] = self.predict
-
-        # Sample the first frame of data to get position columns, if needed
-        args = list(args)
-        frames = iter(args[0])
-        f0 = next(frames)
-        args[0] = itertools.chain([f0], frames)
-
-        # Sort out pos_columns, which must match what the linker is using.
-        # The user may have already specified it, especially if they are giving
-        # an initial guess to a velocity predictor. If so, make sure that the
-        # value given to the linker matches.
-        if getattr(self, 'pos_columns', None) is not None:
-            pos_columns = self.pos_columns
-            if 'pos_columns' in kw and kw['pos_columns'] is not None and any(
-                    [spc != ppc for (spc, ppc) in
-                     zip(pos_columns, kw['pos_columns'])]):
-                    raise ValueError('The optional pos_columns given to the linker '
-                                     'conflicts with the pos_columns used to initialize '
-                                     'this predictor.')
-        else:
-            # If no explicit pos_columns has been given anywhere, now is the time
-            # to guess.
-            pos_columns = kw.get('pos_columns', guess_pos_columns(f0))
-            self.pos_columns = pos_columns
-        # No matter what, ensure that the linker uses the same pos_columns.
-        # (This maintains compatibility with the legacy linkers)
-        kw['pos_columns'] = self.pos_columns
-
+        self.pos_columns = kw.get('pos_columns', ['x', 'y'])
         self.t_column = kw.get('t_column', 'frame')
-        for frame in linking_fcn(*args, **kw):
+        for frame in linking.link_df_iter(*args, **kw):
             self.observe(frame)
             yield frame
 
-    def wrap_single(self, linking_fcn, *args, **kw):
-        """Wrapper for an arbitrary linking function that causes it to use this predictor.
-
-        This wrapper causes the linker to accept and return a single DataFrame
-        with coordinates for all frames. Because it wraps functions that use
-        iterators of DataFrames, it should not necessarily be considered a drop-in replacement
-        for another single-DataFrame linking function.
-
-        The linking function must accept a 'predictor' keyword argument. It
-        must return an iterator of DataFrames, emitting a DataFrame each time
-        a frame is linked.
-        """
-        # TODO: Properly handle empty frames by adopting more sophisticated
-        # logic in e.g. linking._gen_levels_df()
-        args = list(args)
-        features = args.pop(0)
-        if kw.get('t_column') is None:
-            kw['t_column'] = 'frame'
-        kw['predictor'] = self.predict
-        features_iter = (frame for fnum, frame in features.groupby(kw['t_column']))
-        return pandas_concat(self.wrap(linking_fcn, features_iter, *args, **kw))
-
-    def link_df_iter(self, *args, **kw):
-        """Wrapper for linking.link_df_iter() that causes it to use this predictor."""
-        return self.wrap(linking.link_df_iter, *args, **kw)
-
-    def link_df(self, *args, **kw):
-        """Wrapper for linking.link_df_iter() that causes it to use this predictor.
-
-        As with linking.link_df(), the features data is a single DataFrame.
-
-        Note that this does not wrap linking.link_df(), and does not accept the same
-        options as that function. However in most cases it is functionally equivalent.
-        """
-        return self.wrap_single(linking.link_df_iter, *args, **kw)
-
     def observe(self, frame):
         """Examine the latest output of the linker, to update our predictions."""
         pass
 
     def state(self):
         """Return a representation of the predictor's internal state.
 
@@ -131,108 +62,80 @@
         """
         return None
 
     def predict(self, t1, particles):
         """Predict the positions of 'particles' at time 't1'"""
         return map(lambda p: p.pos, particles)
 
-
 class _RecentVelocityPredict(NullPredict):
-    def __init__(self, span=1, pos_columns=None):
-        """Use the 'span'+1 most recent frames to make a velocity field.
-
-        pos_columns should be specified if you will not be using the
-        link_df() or link_df_iter() method for linking with prediction.
-        """
+    def __init__(self, span=1):
+        """Use the 'span'+1 most recent frames to make a velocity field."""
         self.recent_frames = deque([], span + 1)
-        self.pos_columns = pos_columns
 
     def state(self):
         return list(self.recent_frames)
 
-    def _check_pos_columns(self):
-        """Depending on how the predictor is used, it's possible for pos_columns to be missing.
-        This raises a helpful error message in that case."""
-        if self.pos_columns is None:
-            raise AttributeError('If you are not using the link_df() or link_df_iter() methods of the predictor, '
-                                 'you must specify pos_columns when you initialize the predictor object.')
-
     def _compute_velocities(self, frame):
         """Compute velocity field based on a newly-tracked frame."""
-        self._check_pos_columns()
         pframe = frame.set_index('particle')
         self.recent_frames.append(pframe)
         if len(self.recent_frames) == 1:
             # Double the first frame. Velocity field will be zero.
             self.recent_frames.append(pframe)
             dt = 1. # Avoid dividing by zero
         else: # Not the first frame
-            dt = float(self.recent_frames[-1][self.t_column].values[0] -
+            dt = (self.recent_frames[-1][self.t_column].values[0] -
                  self.recent_frames[0][self.t_column].values[0])
 
         # Compute velocity field
         disps = self.recent_frames[-1][self.pos_columns].join(
             self.recent_frames[-1][self.pos_columns] -
                 self.recent_frames[0][self.pos_columns], rsuffix='_disp_').dropna()
         positions = disps[self.pos_columns]
         vels = disps[[cn + '_disp_' for cn in self.pos_columns]] / dt
         # 'vels' will have same column names as 'positions'
-        vels = vels.rename(columns=lambda n: n[:-6])
+        vels.rename(columns=lambda n: n[:-6], inplace=True)
         return dt, positions, vels
 
-
 class NearestVelocityPredict(_RecentVelocityPredict):
     """Predict a particle's position based on the most recent nearby velocity.
 
     Parameters
     ----------
     initial_guess_positions : Nxd array, optional
-        Columns should be in the same order used by the linking function.
     initial_guess_vels : Nxd array, optional
         If specified, these initialize the velocity field with velocity
         samples at the given points.
-    pos_columns : list of d strings, optional
-        Names of coordinate columns corresponding to the columns of
-        the initial_guess arrays, e.g. ['y', 'x']. Required if a guess
-        is specified.
     span : integer, default 1
         Compute velocity field from the most recent span+1 frames.
     """
 
     def __init__(self, initial_guess_positions=None,
-                 initial_guess_vels=None, pos_columns=None, span=1):
-        if initial_guess_positions is not None and pos_columns is None:
-            raise ValueError('The order of the position columns in your initial '
-                             "guess is ambiguous. Specify the coordinate names "
-                             "with your guess, using e.g. pos_columns=['y', 'x']")
-        super().__init__(span=span, pos_columns=pos_columns)
+                 initial_guess_vels=None, span=1):
+        super(NearestVelocityPredict, self).__init__(span=span)
         if initial_guess_positions is not None:
             self.use_initial_guess = True
             self.interpolator = NearestNDInterpolator(
                 np.asarray(initial_guess_positions),
                 np.asarray(initial_guess_vels))
         else:
             self.use_initial_guess = False
 
     def observe(self, frame):
         dt, positions, vels = self._compute_velocities(frame)
         if self.use_initial_guess:
             self.use_initial_guess = False
         else:
             if positions.values.shape[0] > 0:
-                self.interpolator = NearestNDInterpolator(
-                    positions[self.pos_columns].values,
-                    vels[self.pos_columns].values)
+                self.interpolator = NearestNDInterpolator(positions.values, vels.values)
             else:
                 # Sadly, the 2 most recent frames had no points in common.
                 warn('Could not generate velocity field for prediction: no tracks')
-
                 def null_interpolator(*x):
                     return np.zeros((len(x),))
-
                 self.interpolator = null_interpolator
 
     def state(self):
         return {'recent_frames': list(self.recent_frames),
                 'interpolator': self.interpolator,
                 'using_initial_guess': self.use_initial_guess,
                 }
@@ -240,35 +143,25 @@
     def predict(self, t1, particles):
         poslist, tlist = zip(*[(p.pos, p.t) for p in particles])
         positions = np.array(poslist)
         times = np.array(tlist)
         return (positions + self.interpolator(positions) *
                np.tile(t1 - times, (positions.shape[1], 1)).T)
 
-
 class DriftPredict(_RecentVelocityPredict):
     """Predict a particle's position based on the mean velocity of all particles.
 
     Parameters
     ----------
-    initial_guess : Array of length d, optional
-        Velocity vector initially used for prediction.
-        Default is to assume zero velocity.
-    pos_columns : list of d strings, optional
-        Names of coordinate columns corresponding to the elements of
-        initial_guess, e.g. ['y', 'x']. Required if a guess is specified.
+    initial_guess : Array of length d. Otherwise assumed to be zero velocity.
     span : integer, default 1
         Compute velocity field from the most recent span+1 frames.
     """
-    def __init__(self, initial_guess=None, pos_columns=None, span=1):
-        if initial_guess is not None and pos_columns is None:
-            raise ValueError('The order of the position columns in your initial '
-                             "guess is ambiguous. Specify the coordinate names "
-                             "with your guess, using e.g. pos_columns=['y', 'x']")
-        super().__init__(pos_columns=pos_columns, span=span)
+    def __init__(self, initial_guess=None, span=1):
+        super(DriftPredict, self).__init__(span=span)
         self.initial_guess = initial_guess
 
     def observe(self, frame):
         dt, positions, vels = self._compute_velocities(frame)
         if self.initial_guess is not None:
             self.vel = np.asarray(self.initial_guess)
             self.initial_guess = None
@@ -276,16 +169,15 @@
             self.vel = vels.mean().values
 
     def predict(self, t1, particles):
         poslist, tlist = zip(*[(p.pos, p.t) for p in particles])
         positions = np.array(poslist)
         times = np.array(tlist)
         return (positions + self.vel *
-                np.tile(t1 - times, (positions.shape[1], 1)).T)
-
+               np.tile(t1 - times, (positions.shape[1], 1)).T)
 
 class ChannelPredict(_RecentVelocityPredict):
     """Predict a particle's position based on its spanwise coordinate in a channel.
 
     This operates by binning particles according to their spanwise coordinate and
     averaging velocity, to make an instantaneous velocity profile.
 
@@ -297,36 +189,35 @@
     minsamples : Minimum number of particles in a bin for its average
         velocity to be valid.
     initial_profile_guess : Nx2 array (optional)
         (spanwise coordinate, streamwise velocity) samples specifying
         initial velocity profile. Samples must be sufficiently dense to account
         for variation in the velocity profile. If omitted, initial velocities are
         assumed to be zero.
-    pos_columns : list of d strings, optional
-        Names of coordinate columns. Required only if not using link_df or link_df_iter.
     span : integer, default 1
         Compute velocity field from the most recent span+1 frames.
 
     Notes
     -----
     - This currently only works for 2D data.
     - Where there were not enough data to make an average velocity (N < minsamples),
         we borrow from the nearest valid bin.
     """
     def __init__(self, bin_size, flow_axis='x', minsamples=20,
-                 initial_profile_guess=None, pos_columns=None, span=1):
-        super().__init__(pos_columns=pos_columns, span=span)
+                 initial_profile_guess=None, span=1):
+        super(ChannelPredict, self).__init__(span=span)
         self.bin_size = bin_size
         self.flow_axis = flow_axis
         self.minsamples = minsamples
+        # Use the last 2 frames to make a velocity field
+        self.recent_frames = deque([], 2)
         self.initial_profile_guess = initial_profile_guess
 
     def observe(self, frame):
         # Sort out dimensions and axes
-        self._check_pos_columns()
         if len(self.pos_columns) != 2:
             raise ValueError('Implemented for 2 dimensions only')
         if self.flow_axis not in self.pos_columns:
             raise ValueError('pos_columns (%r) does not include the specified flow_axis (%s)!' %
                              (self.pos_columns, self.flow_axis))
         poscols = self.pos_columns[:]
         flow_axis_position = poscols.index(self.flow_axis)
@@ -334,15 +225,15 @@
         span_axis = poscols[0]
 
         # Make velocity profile
         dt, positions, vels = self._compute_velocities(frame)
 
         if self.initial_profile_guess is not None:
             ipg = np.asarray(self.initial_profile_guess)
-            prof = pd.Series(ipg[:, 1], index=ipg[:, 0])
+            prof = pd.Series(ipg[:,1], index=ipg[:,0])
             self.initial_profile_guess = None  # Don't reuse
         else:
             # Bin centers
             vels['bin'] = (positions[span_axis] - positions[span_axis]
                                                  % self.bin_size + self.bin_size / 2.)
             grpvels = vels.groupby('bin')[self.flow_axis]
             # Only use bins that have enough samples
@@ -357,26 +248,24 @@
             prof_vals.insert(0, prof.values[0])
             prof_vals.append(prof.values[-1])
             prof_vels = pd.DataFrame({self.flow_axis: pd.Series(prof_vals, index=prof_ind),
                                       span_axis: 0})
             prof_interp = interp1d(prof_vels.index.values, prof_vels[self.pos_columns].values,
                                    'nearest', axis=0)
             if flow_axis_position == 0:
-                self.interpolator = lambda x: prof_interp(x[:, 1])
+                self.interpolator = lambda x: prof_interp(x[:,1])
             else:
-                self.interpolator = lambda x: prof_interp(x[:, 0])
+                self.interpolator = lambda x: prof_interp(x[:,0])
         else:
             # Not enough samples in any bin
             warn('Could not generate velocity field for prediction: '
                  'not enough tracks or bin_size too small')
             nullvel = np.zeros((len(self.pos_columns),))
-
             def null_interpolator(x):
                 return nullvel
-
             self.interpolator = null_interpolator
 
     def state(self):
         return {'recent_frames': list(self.recent_frames),
                 'interpolator': self.interpolator,
                 'initial_profile_guess': self.initial_profile_guess,
                 }
@@ -384,48 +273,45 @@
     def predict(self, t1, particles):
         poslist, tlist = zip(*[(p.pos, p.t) for p in particles])
         positions = np.array(poslist)
         times = np.array(tlist)
         return (positions + self.interpolator(positions) *
                np.tile(t1 - times, (positions.shape[1], 1)).T)
 
-
 def instrumented(limit=None):
     """Decorate a predictor class and allow it to record inputs and outputs.
 
     Use when diagnosing prediction.
 
     limit : maximum number of recent frames to retain. If None, keep all.
 
-    Examples
-    --------
-
-    >>> pred = instrumented()(ChannelPredict)(50, flow_axis='y')
-    >>> pred.link_df_iter(...)
-    >>> diagnostics = pred.dump()
+    Example:
+        pred = instrumented()(ChannelPredict)(50, flow_axis='y')
+        pred.link_df_iter(...)
+        diagnostics = pred.dump()
     """
     def instrumentor(cls):
         class InstrumentedPredictor(cls):
             def __init__(self, *args, **kw):
-                super().__init__(*args, **kw)
+                super(InstrumentedPredictor, self).__init__(*args, **kw)
                 self.diag_observations = deque([], maxlen=limit)
                 self.diag_predictions = deque([], maxlen=limit)
 
             def observe(self, frame):
                 self.diag_observations.append(frame)
-                return super().observe(frame)
+                return super(InstrumentedPredictor, self).observe(frame)
 
             def predict(self, t1, particles):
                 poslist, tlist, tracklist = zip(*[
                     (p.pos, p.t, p.track.id) for p in particles])
                 pdf = pd.DataFrame(np.array(poslist), columns=self.pos_columns)
                 pdf[self.t_column] = tlist
                 pdf['particle'] = np.array(tracklist, dtype=int)
 
-                prediction = super().predict(t1, particles)
+                prediction = super(InstrumentedPredictor, self).predict(t1, particles)
                 pred_df = pd.DataFrame(prediction, columns=self.pos_columns)
                 dd = {'t1': t1,
                       'particledf': pdf.join(pred_df, rsuffix='_pred'),
                       'state': self.state()}
                 self.diag_predictions.append(dd)
 
                 return prediction
@@ -454,7 +340,9 @@
                         on='particle', rsuffix='_act')
                     results.append(dd)
                 results.reverse()  # Back to chronological order
                 return results
 
         return InstrumentedPredictor
     return instrumentor
+
+
```

### Comparing `trackpy-0.6.3rc1/trackpy/utils.py` & `trackpy-unknown/trackpy/plots.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,430 +1,409 @@
-import logging
-import functools
-import re
-import sys
-import warnings
-from collections.abc import Hashable
-from datetime import datetime, timedelta
-from looseversion import LooseVersion
-from multiprocessing.pool import Pool
+"""These functions generate handy plots."""
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
+import six
+from six.moves import zip
+from itertools import tee
+from collections import Iterable
+from functools import wraps
 
-import pandas as pd
 import numpy as np
-import scipy
-from scipy import stats
-import yaml
-
-import trackpy
-
-
-try:
-    is_pandas_since_023 = (LooseVersion(pd.__version__) >=
-                           LooseVersion('0.23.0'))
-except ValueError:  # Probably a development version
-    is_pandas_since_023 = True
-
-# Emit warnings in refine.least_squares for scipy 1.5
-try:
-    is_scipy_15 = LooseVersion("1.5.0") <= LooseVersion(scipy.__version__) < LooseVersion('1.6.0')
-except ValueError:  # Probably a development version
-    is_scipy_15 = False
-
-
-def fit_powerlaw(data, plot=True, **kwargs):
-    """Fit a powerlaw by doing a linear regression in log space."""
-    ys = pd.DataFrame(data)
-    x = pd.Series(data.index.values, index=data.index, dtype=np.float64)
-    values = pd.DataFrame(index=['n', 'A'])
-    fits = {}
-    for col in ys:
-        y = ys[col].dropna()
-        slope, intercept, r, p, stderr = \
-            stats.linregress(np.log(x), np.log(y))
-        values[col] = [slope, np.exp(intercept)]
-        fits[col] = x.apply(lambda x: np.exp(intercept)*x**slope)
-    values = values.T
-    fits = pandas_concat(fits, axis=1)
-    if plot:
-        from trackpy import plots
-        plots.fit(data, fits, logx=True, logy=True, legend=False, **kwargs)
-    return values
-
-
-class memo:
-    """Decorator. Caches a function's return value each time it is called.
-    If called later with the same arguments, the cached value is returned
-    (not reevaluated).
-    http://wiki.python.org/moin/PythonDecoratorLibrary#Memoize """
-    def __init__(self, func):
-        self.func = func
-        self.cache = {}
-        functools.update_wrapper(self, func)
-
-    def __call__(self, *args):
-        if not isinstance(args, Hashable):
-            # uncacheable. a list, for instance.
-            warnings.warn("A memoization cache is being used on an uncacheable " +
-                          "object. Proceeding by bypassing the cache.",
-                          UserWarning)
-            return self.func(*args)
-        if args in self.cache:
-            return self.cache[args]
-        else:
-            value = self.func(*args)
-            self.cache[args] = value
-            return value
-# This code trips up numba. It's nice for development
-# but it shouldn't matter for users.
-#   def __repr__(self):
-#      '''Return the function's docstring.'''
-#      return self.func.__doc__
-
-    def __get__(self, obj, objtype):
-        '''Support instance methods.'''
-        return functools.partial(self.__call__, obj)
-
-
-def extract(pattern, string, group, convert=None):
-    """Extract a pattern from a string. Optionally, convert it
-    to a desired type (float, timestamp, etc.) by specifying a function.
-    When the pattern is not found, gracefully return None."""
-    # group may be 1, (1,) or (1, 2).
-    if type(group) is int:
-        grp = (group,)
-    elif type(group) is tuple:
-        grp = group
-    assert type(grp) is tuple, "The arg 'group' should be an int or a tuple."
-    try:
-        result = re.search(pattern, string, re.DOTALL).group(*grp)
-    except AttributeError:
-        # For easy unpacking, when a tuple is expected, return a tuple of Nones.
-        return None if type(group) is int else (None,)*len(group)
-    return convert(result) if convert else result
-
-
-def timestamp(ts_string):
-    "Convert a timestamp string to a datetime type."
-    if ts_string is None:
-        return None
-    return datetime.strptime(ts_string, '%Y-%m-%d %H:%M:%S')
-
-
-def time_interval(raw):
-    "Convert a time interval string into a timedelta type."
-    if raw is None:
-        return None
-    m = re.match('([0-9][0-9]):([0-5][0-9]):([0-5][0-9])', raw)
-    h, m, s = map(int, m.group(1, 2, 3))
-    return timedelta(hours=h, minutes=m, seconds=s)
-
-
-def suppress_plotting():
-    import matplotlib.pyplot as plt
-    plt.switch_backend('Agg') # does not plot to screen
+import pandas as pd
+from pandas import DataFrame, Series
 
+from .utils import print_update
 
-# HH:MM:SS, H:MM:SS, MM:SS, M:SS all OK
-lazy_timestamp_pat = r'\d?\d?:?\d?\d:\d\d'
 
-# a time stamp followed by any text comment
-ltp = lazy_timestamp_pat
-video_log_pattern = r'(' + ltp + r')-?(' + ltp + r')? ?(RF)?(.+)?'
+def make_axes(func):
+    """
+    A decorator for plotting functions.
+    NORMALLY: Direct the plotting function to the current axes, gca().
+              When it's done, make the legend and show that plot.
+              (Instant gratificaiton!)
+    BUT:      If the uses passes axes to plotting function, write on those axes
+              and return them. The user has the option to draw a more complex
+              plot in multiple steps.
+    """
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        import matplotlib as mpl
+        import matplotlib.pyplot as plt
+        if kwargs.get('ax') is None:
+            kwargs['ax'] = plt.gca()
+            # Delete legend keyword so remaining ones can be passed to plot().
+            try:
+                legend = kwargs['legend']
+            except KeyError:
+                legend = None
+            else:
+                del kwargs['legend']
+            result = func(*args, **kwargs)
+            if not (kwargs['ax'].get_legend_handles_labels() == ([], []) or \
+                    legend is False):
+                plt.legend(loc='best')
+            plt.show()
+            return result
+        else:
+            return func(*args, **kwargs)
+    return wrapper
 
+def make_fig(func):
+    """See make_axes."""
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+    wraps(func)
+    def wrapper(*args, **kwargs):
+        if 'fig' not in kwargs:
+            kwargs['fig'] = plt.gcf()
+            func(*args, **kwargs)
+            plt.show()
+        else:
+            return func(*args, **kwargs)
+    return wrapper
 
-def lazy_timestamp(partial_timestamp):
-    """Regularize a lazy timestamp like '0:37' -> '00:00:37'.
-HH:MM:SS, H:MM:SS, MM:SS, and M:SS all OK.
+@make_axes
+def plot_traj(traj, colorby='particle', mpp=None, label=False,
+              superimpose=None, cmap=None, ax=None, t_column=None,
+              **kwargs):
+    """Plot traces of trajectories for each particle.
+    Optionally superimpose it on a frame from the video.
 
     Parameters
     ----------
-    partial_timestamp : string or other object
+    traj : DataFrame including columns x and y
+    colorby : {'particle', 'frame'}
+    mpp : microns per pixel
+        If omitted, the labels will be labeled in units of pixels.
+    label : Set to True to write particle ID numbers next to trajectories.
+    superimpose : background image, default None
+    cmap : This is only used in colorby='frame' mode.
+        Default = mpl.cm.winter
+    ax : matplotlib axes object, defaults to current axes
+    t_column : DataFrame column name
+        Default is 'frame'
 
     Returns
     -------
-    regularized string
+    None
     """
-    if not isinstance(partial_timestamp, str):
-        # might be NaN or other unprocessable entry
-        return partial_timestamp
-    input_format = r'\d?\d?:?\d?\d:\d\d'
-    if not re.match(input_format, partial_timestamp):
-        raise ValueError("Input string cannot be regularized.")
-    partial_digits = list(partial_timestamp)
-    digits = ['0', '0', ':', '0', '0', ':', '0', '0']
-    digits[-len(partial_digits):] = partial_digits
-    return ''.join(digits)
-
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+    from matplotlib.collections import LineCollection
 
-def timedelta_to_frame(timedeltas, fps):
-    """Convert timedelta times into frame numbers.
+    if cmap is None:
+        cmap = plt.cm.winter
+    if t_column is None:
+        t_column = 'frame'
+
+    # Axes labels
+    if mpp is None:
+        ax.set_xlabel('x [px]')
+        ax.set_ylabel('y [px]')
+        mpp = 1.  # for computations of image extent below
+    else:
+        if mpl.rcParams['text.usetex']:
+            ax.set_xlabel(r'x [\textmu m]')
+            ax.set_ylabel(r'y [\textmu m]')
+        else:
+            ax.set_xlabel('x [\xb5m]')
+            ax.set_ylabel('y [\xb5m]')
+    # Background image
+    if superimpose is not None:
+        ax.imshow(superimpose, cmap=plt.cm.gray,
+                  origin='lower', interpolation='none',
+                  vmin=kwargs.get('vmin'), vmax=kwargs.get('vmax'))
+        ax.set_xlim(-0.5 * mpp, (superimpose.shape[1] - 0.5) * mpp)
+        ax.set_ylim(-0.5 * mpp, (superimpose.shape[0] - 0.5) * mpp)
+    # Trajectories
+    if colorby == 'particle':
+        # Unstack particles into columns.
+        unstacked = traj.set_index([t_column, 'particle']).unstack()
+        ax.plot(mpp*unstacked['x'], mpp*unstacked['y'], linewidth=1)
+    if colorby == 'frame':
+        # Read http://www.scipy.org/Cookbook/Matplotlib/MulticoloredLine
+        x = traj.set_index([t_column, 'particle'])['x'].unstack()
+        y = traj.set_index([t_column, 'particle'])['y'].unstack()
+        color_numbers = traj[t_column].values/float(traj[t_column].max())
+        print_update("Drawing multicolor lines takes awhile. "
+                     "Come back in a minute.")
+        for particle in x:
+            points = np.array(
+                [x[particle].values, y[particle].values]).T.reshape(-1, 1, 2)
+            segments = np.concatenate([points[:-1], points[1:]], axis=1)
+            lc = LineCollection(segments, cmap=cmap)
+            lc.set_array(color_numbers)
+            ax.add_collection(lc)
+            ax.set_xlim(x.apply(np.min).min(), x.apply(np.max).max())
+            ax.set_ylim(y.apply(np.min).min(), y.apply(np.max).max())
+    if label:
+        unstacked = traj.set_index([t_column, 'particle'])[['x', 'y']].unstack()
+        first_frame = int(traj[t_column].min())
+        coords = unstacked.fillna(method='backfill').stack().loc[first_frame]
+        for particle_id, coord in coords.iterrows():
+            plt.text(coord['x'], coord['y'], "%d" % particle_id,
+                     horizontalalignment='center',
+                     verticalalignment='center')
+    ax.invert_yaxis()
+    return ax
+
+ptraj = plot_traj # convenience alias
+
+@make_axes
+def annotate(centroids, image, circle_size=None, color=None,
+             invert=False, ax=None, split_category=None, split_thresh=None,
+             imshow_style={}, plot_style={}):
+    """Mark identified features with white circles.
 
     Parameters
     ----------
-    timedelta : DataFrame or Series of timedelta64 datatype
-    fps : frames per second (integer)
-
-    Result
+    centroids : DataFrame including columns x and y
+    image : image array (or string path to image file)
+    circle_size : Deprecated.
+        This will be removed in a future version of trackpy.
+        Use `plot_style={'markersize': ...}` instead.
+    color : single matplotlib color or a list of multiple colors
+        default None
+    invert : If you give a filepath as the image, specify whether to invert
+        black and white. Default True.
+    ax : matplotlib axes object, defaults to current axes
+    split_category : string, parameter to use to split the data into sections
+        default None
+    split_thresh : single value or list of ints or floats to split 
+        particles into sections for plotting in multiple colors.
+        List items should be ordered by increasing value.
+        default None
+    imshow_style : dictionary of keyword arguments passed through to
+        the `Axes.imshow(...)` command the displays the image
+    plot_style : dictionary of keyword arguments passed through to
+        the `Axes.plot(...)` command that marks the features
+    
+    Returns
     ------
-    DataFrame
-
-    Note
-    ----
-    This sounds like a stupidly easy operation, but handling missing data
-    and multiplication is tricky with timedeltas.
-    """
-    ns = timedeltas.values
-    seconds = ns * 1e-9
-    frame_numbers = seconds*fps
-    result = pd.DataFrame(frame_numbers, dtype=np.int64,
-                          index=timedeltas.index, columns=timedeltas.columns)
-    result = result.where(timedeltas.notnull(), np.nan)
-    return result
-
-
-def random_walk(N):
-    return np.cumsum(np.random.randn(N), 1)
-
-
-def record_meta(meta_data, file_obj):
-    file_obj.write(yaml.dump(meta_data, default_flow_style=False))
-
-def validate_tuple(value, ndim):
-    if not hasattr(value, '__iter__'):
-        return (value,) * ndim
-    if len(value) == ndim:
-        return tuple(value)
-    raise ValueError("List length should have same length as image dimensions.")
-
-
-try:
-    from IPython.display import clear_output
-except ImportError:
-    pass
-
-
-def make_pandas_strict():
-    """Configure Pandas to raise an exception for "chained assignments."
-
-    This is useful during tests.
-    See http://pandas.pydata.org/pandas-docs/stable/indexing.html#indexing-view-versus-copy
-
-    Does nothing for Pandas versions before 0.13.0.
-    """
-    if LooseVersion(pd.__version__) >= LooseVersion('0.13.0'):
-        pd.set_option('mode.chained_assignment', 'raise')
-
-
-class IPythonStreamHandler(logging.StreamHandler):
-    "A StreamHandler for logging that clears output between entries."
-    def emit(self, s):
-        clear_output(wait=True)
-        print(s.getMessage())
-    def flush(self):
-        sys.stdout.flush()
-
-
-FORMAT = "%(name)s.%(funcName)s:  %(message)s"
-formatter = logging.Formatter(FORMAT)
-
-# Check for IPython and use a special logger
-use_ipython_handler = False
-try:
-    import IPython
-except ImportError:
-    pass
-else:
-    if IPython.get_ipython() is not None:
-        use_ipython_handler = True
-if use_ipython_handler:
-    default_handler = IPythonStreamHandler()
-else:
-    default_handler = logging.StreamHandler(sys.stdout)
-default_handler.setLevel(logging.INFO)
-default_handler.setFormatter(formatter)
-
-
-def handle_logging():
-    "Send INFO-level log messages to stdout. Do not propagate."
-    if use_ipython_handler:
-        # Avoid double-printing messages to IPython stderr.
-        trackpy.logger.propagate = False
-    trackpy.logger.addHandler(default_handler)
-    trackpy.logger.setLevel(logging.INFO)
-
-
-def ignore_logging():
-    "Reset to factory default logging configuration; remove trackpy's handler."
-    trackpy.logger.removeHandler(default_handler)
-    trackpy.logger.setLevel(logging.NOTSET)
-    trackpy.logger.propagate = True
-
-
-def quiet(suppress=True):
-    """Suppress trackpy information log messages.
-
-    Parameters
-    ----------
-    suppress : boolean
-        If True, set the logging level to WARN, hiding INFO-level messages.
-        If False, set level to INFO, showing informational messages.
-    """
-    if suppress:
-        trackpy.logger.setLevel(logging.WARN)
-    else:
-        trackpy.logger.setLevel(logging.INFO)
-
-
-def pandas_sort(df, by, *args, **kwargs):
+    axes
     """
-    Use sort_values() to sort a DataFrame
-    This raises a ValueError if the given value is both
-    a column and an index label, i.e.:
-    ValueError: 'frame' is both an index level and a column
-    label, which is ambiguous.
-    Because we usually sort by columns, we can rename
-    the index to supress the ValueError.
-    """
-    if df.index.name is not None and df.index.name in by:
-        df.index.name += '_index'
-    return df.sort_values(*args, by=by, **kwargs)
-
-
-def _pandas_concat_post_023(*args, **kwargs):
-    """Pass sort = False. Breaks API by not sorting, but we don't care. """
-    kwargs.setdefault('sort', False)
-    return pd.concat(*args, **kwargs)
-
-if is_pandas_since_023:
-    pandas_concat = _pandas_concat_post_023
-else:
-    pandas_concat = pd.concat
-
-
-def guess_pos_columns(f):
-    """ Guess the position columns from a given feature DataFrame """
-    if 'z' in f:
-        pos_columns = ['z', 'y', 'x']
-    else:
-        pos_columns = ['y', 'x']
-    return pos_columns
+    import matplotlib.pyplot as plt
 
+    if circle_size is not None:
+        warnings.warn("circle_size will be removed in future version of "
+                      "trackpy. Use plot_style={'markersize': ...} instead.")
+        if 'marker_size' not in plot_style:
+            plot_style['marker_size'] = np.sqrt(circle_size)  # area vs. dia.
+        else:
+            raise ValueError("passed in both 'marker_size' and 'circle_size'") 
 
-def default_pos_columns(ndim):
-    """ Sets the default position column names """
-    if ndim < 4:
-        return ['z', 'y', 'x'][-ndim:]
+    _plot_style = dict(markersize=15, markeredgewidth=2,
+                       markerfacecolor='none', markeredgecolor='r',
+                       marker='o', linestyle='none')
+    _plot_style.update(**_normalize_kwargs(plot_style, 'line2d'))
+    _imshow_style = dict(origin='lower', interpolation='none',
+                         cmap=plt.cm.gray)
+    _imshow_style.update(imshow_style)
+
+    # https://docs.python.org/2/library/itertools.html
+    def pairwise(iterable):
+        "s -> (s0,s1), (s1,s2), (s2, s3), ..."
+        a, b = tee(iterable)
+        next(b, None)
+        return zip(a, b)
+
+    if color is None:
+        color = ['r']
+    if isinstance(color, six.string_types):
+        color = [color]
+    if not isinstance(split_thresh, Iterable):
+        split_thresh = [split_thresh]
+
+    # The parameter image can be an image object or a filename.
+    if isinstance(image, six.string_types):
+        image = plt.imread(image)
+    if invert:
+        ax.imshow(1-image, **_imshow_style)
     else:
-        return list(map(lambda i: 'x' + str(i), range(ndim)))
-
-
-def default_size_columns(ndim, isotropic):
-    """ Sets the default size column names """
-    if isotropic:
-        return ['size']
+        ax.imshow(image, **_imshow_style)
+    ax.set_xlim(-0.5, image.shape[1] - 0.5)
+    ax.set_ylim(-0.5, image.shape[0] - 0.5)
+
+    if split_category is None:
+        if np.size(color) > 1:
+            raise ValueError("multiple colors specified, no split category "
+                             "specified")
+        _plot_style.update(markeredgecolor=color[0])
+        ax.plot(centroids['x'], centroids['y'],
+                **_plot_style)
     else:
-        return ['size_' + cc for cc in default_pos_columns(ndim)]
-
+        if len(color) != len(split_thresh) + 1:
+            raise ValueError("number of colors must be number of thresholds "
+                             "plus 1")
+        low = centroids[split_category] < split_thresh[0]
+        _plot_style.update(markeredgecolor=color[0])
+        ax.plot(centroids['x'][low], centroids['y'][low], 
+                **_plot_style)
+
+        for c, (bot, top) in zip(color[1:-1], pairwise(split_thresh)):
+            indx = ((centroids[split_category] >= bot) &
+                    (centroids[split_category] < top))
+            _plot_style.update(markeredgecolor=c)
+            ax.plot(centroids['x'][indx], centroids['y'][indx], 
+                    **_plot_style)
+
+        high = centroids[split_category] >= split_thresh[-1]
+        _plot_style.update(markeredgecolor=color[-1])
+        ax.plot(centroids['x'][high], centroids['y'][high], 
+                **_plot_style)
+    return ax
+
+
+@make_axes
+def mass_ecc(f, ax=None):
+    """Plot each particle's mass versus eccentricity."""
+    ax.plot(f['mass'], f['ecc'], 'ko', alpha=0.3)
+    ax.set_xlabel('mass')
+    ax.set_ylabel('eccentricity (0=circular)')
+    return ax
+
+@make_axes
+def mass_size(f, ax=None):
+    """Plot each particle's mass versus size."""
+    ax.plot(f['mass'], f['size'], 'ko', alpha=0.1)
+    ax.set_xlabel('mass')
+    ax.set_ylabel('size')
+    return ax
+
+@make_axes
+def subpx_bias(f, ax=None):
+    """Histogram the fractional part of the x and y position.
+
+    Notes
+    -----
+    If subpixel accuracy is good, this should be flat. If it depressed in the
+    middle, try using a larger value for feature diameter."""
+    f[['x', 'y']].applymap(lambda x: x % 1).hist(ax=ax)
+    return ax
+
+@make_axes
+def fit(data, fits, inverted_model=False, logx=False, logy=False, ax=None,
+        **kwargs):
+    import matplotlib.pyplot as plt
 
-def is_isotropic(value):
-    """ Determine whether all elements of a value are equal """
-    if hasattr(value, '__iter__'):
-        return np.all(value[1:] == value[:-1])
+    data = data.dropna()
+    x, y = data.index.values.astype('float64'), data.values
+    datalines = plt.plot(x, y, 'o', label=data.name, **kwargs)
+    ax = datalines[0].get_axes()
+    if logx:
+        ax.set_xscale('log')
+    if logy:
+        ax.set_yscale('log')
+    if not inverted_model:
+        fitlines = ax.plot(fits.index, fits, **kwargs)
     else:
-        return True
-
+        fitlines = ax.plot(fits.reindex(data.dropna().index),
+                           data.dropna(), **kwargs)
+    # Restrict plot axis to domain of the data, not domain of the fit.
+    xmin = data.index.values[data.index.values > 0].min() if logx \
+        else data.index.values.min()
+    ax.set_xlim(xmin, data.index.values.max())
+    # Match colors of data and corresponding fits.
+    [f.set_color(d.get_color()) for d, f in zip(datalines, fitlines)]
+    if logx:
+        ax.set_xscale('log') # logx kwarg does not always take. Bug?
+
+@make_axes
+def plot_principal_axes(img, x_bar, y_bar, cov, ax=None):
+    """Plot bars with a length of 2 stddev along the principal axes.
+
+    Attribution
+    -----------
+    This function is based on a solution by Joe Kington, posted on Stack
+    Overflow at http://stackoverflow.com/questions/5869891/
+    how-to-calculate-the-axis-of-orientation/5873296#5873296
+    """
+    def make_lines(eigvals, eigvecs, mean, i):
+        """Make lines a length of 2 stddev."""
+        std = np.sqrt(eigvals[i])
+        vec = 2 * std * eigvecs[:,i] / np.hypot(*eigvecs[:,i])
+        x, y = np.vstack((mean-vec, mean, mean+vec)).T
+        return x, y
+    mean = np.array([x_bar, y_bar])
+    eigvals, eigvecs = np.linalg.eigh(cov)
+    ax.plot(*make_lines(eigvals, eigvecs, mean, 0), marker='o', color='white')
+    ax.plot(*make_lines(eigvals, eigvecs, mean, -1), marker='o', color='red')
+    ax.imshow(img)
 
-class ReaderCached:
-    """ Simple wrapper that provides cacheing of image readers """
-    def __init__(self, reader):
-        self.reader = reader
-        self._cache = None
-        self._cache_i = None
-
-    def __getitem__(self, i):
-        if self._cache_i == i:
-            return self._cache.copy()
-        else:
-            value = self.reader[i]
-            self._cache = value.copy()
-            return value
-
-    def __repr__(self):
-        return repr(self.reader) + "\nWrapped in ReaderCached"
-
-    def __getattr__(self, attr):
-        return getattr(self.reader, attr)
-
-
-def catch_keyboard_interrupt(gen, logger=None):
-    """ A generator that stops on a KeyboardInterrupt """
-    running = True
-    gen = iter(gen)
-    while running:
-        try:
-            yield next(gen)
-        except KeyboardInterrupt:
-            if logger is not None:
-                logger.warn('KeyboardInterrupt')
-            running = False
-        except StopIteration:
-            running = False
-        else:
-            pass
+def examine_jumps(data, jumps):
+    import matplotlib.pyplot as plt
 
-EXPONENT_EPS_FLOAT64 = np.log(np.finfo(np.float64).eps)
-def safe_exp(arr):
-    # Calculate exponent, dealing with NaN and Underflow warnings
-    result = np.zeros_like(arr)
-    result[np.isnan(arr)] = np.nan  # propagate NaNs
-    with np.errstate(invalid='ignore'):  # ignore comparison with NaN
-        mask = arr > EXPONENT_EPS_FLOAT64
-    result[mask] = np.exp(arr[mask])
-    return result
-
-def get_pool(processes):
-    """Returns the appropriate pool and map functions if multiprocessing needs
-    to be used, otherwise None, map.
+    fig, axes = plt.subplots(len(jumps), 1)
+    for i, jump in enumerate(jumps):
+        roi = data.ix[jump-10:jump+10]
+        axes[i].plot(roi.index, roi, 'g.')
+        axes[i].plot(jump, data[jump], 'ko')
+    fig.show()
+    fig2, axes2 = plt.subplots(1, 1)
+    axes2.plot(data.index, data, 'g.')
+    for jump in jumps:
+        axes2.plot(jump, data[jump], 'ko')
+    fig2.show()
+
+@make_axes
+def plot_displacements(t, frame1, frame2, scale=1, ax=None, **kwargs):
+    """Plot arrows showing particles displacements between two frames.
 
     Parameters
     ----------
-    processes : integer or "auto"
-        The number of processes to use in parallel. If <= 1, multiprocessing is
-        disabled. If "auto", the number returned by `os.cpu_count()`` is used.
-
-    Returns
-    -------
-    pool, map_func
-
-    See Also
-    --------
-    batch
-    """
-    # Handle & validate argument `processes`
-    if processes == "auto":
-        processes = None  # Is replaced with `os.cpu_count` in Pool
-    elif not isinstance(processes, int):
-        raise TypeError("`processes` must either be an integer or 'auto', "
-                        "was type {}".format(type(processes)))
-
-    if processes is None or processes > 1:
-        # Use multiprocessing
-        pool = Pool(processes=processes)
-        map_func = pool.imap
-    else:
-        pool = None
-        map_func = map
-
-    return pool, map_func
-
-
-def stats_mode_scalar(a):
-    """Returns a scalar from scipy.stats.mode().
+    t : DataFrame
+        trajectories, including columns 'frame' and 'particle'
+    frame1 : integer
+        frame number
+    frame2 : integer
+        frame number
+    scale : float
+        scale factor, if 1 (default) then arrow end is placed at particle
+        destination; if any other number arrows are rescaled
+
+    Other Parameters
+    ----------------
+    ax : matplotlib axes (optional)
 
-    See https://docs.scipy.org/doc/scipy-1.9.3/reference/generated/scipy.stats.mode.html
+    Any other keyword arguments will pass through to matplotlib's `annotate`.
     """
-    try:
-        # scipy >= 1.11
-        return stats.mode(a, keepdims=False).mode
-    except TypeError:
-        # Old behavior (keepdims is not accepted)
-        return stats.mode(a).mode[0]
+    a = t[t.frame == frame1]
+    b = t[t.frame == frame2]
+    j= a.set_index('particle')[['x', 'y']].join(
+        b.set_index('particle')[['x', 'y']], rsuffix='_b')
+    j['dx'] = j.x_b - j.x
+    j['dy'] = j.y_b - j.y
+    arrow_specs = j[['x', 'y', 'dx', 'dy']].dropna()
+
+    # Arrow defaults
+    default_arrow_props = dict(arrowstyle='->', connectionstyle='arc3',
+                               linewidth=2)
+    kwargs['arrowprops'] = kwargs.get('arrowprops', default_arrow_props)
+    for _, row in arrow_specs.iterrows():
+        xy = row[['x', 'y']]  # arrow start
+        xytext = xy.values + scale*row[['dx', 'dy']].values  # arrow end
+        # Use ax.annotate instead of ax.arrow because it is allows more
+        # control over arrow style.
+        ax.annotate("",
+                    xy=xy, xycoords='data',
+                    xytext=xytext, textcoords='data',
+                    **kwargs)
+    ax.set_xlim(arrow_specs.x.min(), arrow_specs.x.max())
+    ax.set_ylim(arrow_specs.y.min(), arrow_specs.y.max())
+    return ax
+
+
+def _normalize_kwargs(kwargs, kind='patch'):
+    """Convert matplotlib keywords from short to long form."""
+    # Source:
+    # github.com/tritemio/FRETBursts/blob/fit_experim/fretbursts/burst_plot.py
+    if kind == 'line2d':
+        long_names = dict(c='color', ls='linestyle', lw='linewidth',
+                          mec='markeredgecolor', mew='markeredgewidth',
+                          mfc='markerfacecolor', ms='markersize',)
+    elif kind == 'patch':
+        long_names = dict(c='color', ls='linestyle', lw='linewidth',
+                          ec='edgecolor', fc='facecolor',)
+    for short_name in long_names:
+        if short_name in kwargs:
+            kwargs[long_names[short_name]] = kwargs.pop(short_name)
+    return kwargs
```

