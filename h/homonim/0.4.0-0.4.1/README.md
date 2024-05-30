# Comparing `tmp/homonim-0.4.0.tar.gz` & `tmp/homonim-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homonim-0.4.0.tar", last modified: Thu Feb 22 19:48:14 2024, max compression
+gzip compressed data, was "homonim-0.4.1.tar", last modified: Thu May 30 19:53:19 2024, max compression
```

## Comparing `homonim-0.4.0.tar` & `homonim-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 19:48:14.712903 homonim-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-22 19:48:01.000000 homonim-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-02-22 19:48:14.712903 homonim-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-02-22 19:48:01.000000 homonim-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 19:48:14.708903 homonim-0.4.0/homonim/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30582 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    26452 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/matched_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/raster_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    20334 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/raster_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-22 19:48:01.000000 homonim-0.4.0/homonim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 19:48:14.708903 homonim-0.4.0/homonim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-22 19:48:14.000000 homonim-0.4.0/homonim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-22 19:48:01.000000 homonim-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 19:48:14.712903 homonim-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 19:48:14.708903 homonim-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_fuse_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23171 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_fuse_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_matched_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16786 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_raster_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_raster_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-02-22 19:48:01.000000 homonim-0.4.0/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:53:19.753265 homonim-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-30 19:53:09.000000 homonim-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-30 19:53:19.753265 homonim-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-30 19:53:09.000000 homonim-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:53:19.753265 homonim-0.4.1/homonim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30781 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19971 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26449 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/matched_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26314 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/raster_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20303 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/raster_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 19:53:09.000000 homonim-0.4.1/homonim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:53:19.753265 homonim-0.4.1/homonim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 19:53:19.000000 homonim-0.4.1/homonim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-30 19:53:09.000000 homonim-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:53:19.753265 homonim-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:53:19.753265 homonim-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_fuse_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23171 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_fuse_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_matched_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16786 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_raster_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_raster_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-30 19:53:09.000000 homonim-0.4.1/tests/test_stats.py
```

### Comparing `homonim-0.4.0/LICENSE` & `homonim-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/PKG-INFO` & `homonim-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homonim
-Version: 0.4.0
+Version: 0.4.1
 Summary: Correct aerial and satellite imagery to surface reflectance.
 Author: Leftfield Geospatial
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/leftfield-geospatial/homonim
 Project-URL: Source, https://github.com/leftfield-geospatial/homonim
 Project-URL: Documentation, https://homonim.readthedocs.io
 Project-URL: Changelog, https://github.com/leftfield-geospatial/homonim/releases
@@ -34,15 +34,15 @@
 
 .. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
-Correct aerial and satellite imagery to surface reflectance.
+Correct drone, aerial and satellite imagery to surface reflectance.
 
 .. short_descr_end
 .. description_start
 
 Description
 -----------
 
@@ -138,16 +138,15 @@
 .. comment
     The code below is copied from docs/examples/api_example and # [*] comments removed
 
 .. api_example_start
 
 .. code:: python
 
-    from pathlib import Path
-    from homonim import RasterFuse, RasterCompare, Model
+    from homonim import RasterFuse, Model
 
     # urls of source and reference test images
     src_file = (
         'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
```

### Comparing `homonim-0.4.0/README.rst` & `homonim-0.4.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 .. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
-Correct aerial and satellite imagery to surface reflectance.
+Correct drone, aerial and satellite imagery to surface reflectance.
 
 .. short_descr_end
 .. description_start
 
 Description
 -----------
 
@@ -109,16 +109,15 @@
 .. comment
     The code below is copied from docs/examples/api_example and # [*] comments removed
 
 .. api_example_start
 
 .. code:: python
 
-    from pathlib import Path
-    from homonim import RasterFuse, RasterCompare, Model
+    from homonim import RasterFuse, Model
 
     # urls of source and reference test images
     src_file = (
         'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
```

### Comparing `homonim-0.4.0/homonim/__init__.py` & `homonim-0.4.1/homonim/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,21 @@
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import os
 import pathlib
 import logging
-import warnings
 
-from rasterio.errors import NotGeoreferencedWarning
 from homonim.compare import RasterCompare
 from homonim.enums import Model, ProcCrs
 from homonim.fuse import RasterFuse
 from homonim.kernel_model import KernelModel
 from homonim.stats import ParamStats
 
-# suppress NotGeoreferencedWarning which rasterio can raise incorrectly
-warnings.simplefilter('ignore', category=NotGeoreferencedWarning)
-
 # Add a NullHandler to the package logger to hide logs by default.  Applications can then add
 # their own handler(s).
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 
 if '__file__' in globals():
     root_path = pathlib.Path(__file__).absolute().parents[1]
```

### Comparing `homonim-0.4.0/homonim/cli.py` & `homonim-0.4.1/homonim/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import click
 import cloup
 import numpy as np
 import rasterio as rio
 import yaml
 from click.core import ParameterSource
 from rasterio.warp import SUPPORTED_RESAMPLING
+from rasterio.errors import NotGeoreferencedWarning
 
 from homonim import utils, version, RasterFuse, RasterCompare, ParamStats, ProcCrs, Model
 from homonim.errors import ImageFormatError
 from homonim.raster_array import RasterArray
 from homonim.kernel_model import KernelModel
 
 logger = logging.getLogger(__name__)
@@ -141,14 +142,17 @@
         if file is not None or not is_relative_to:
             orig_show_warning(message, category, filename, lineno, file, line)
         else:
             module_name = module_path.with_suffix('').as_posix().replace('/', '.')
             logger = logging.getLogger(module_name)
             logger.warning(str(message))
 
+    # suppress NotGeoreferencedWarning which rasterio can raise incorrectly
+    warnings.simplefilter('ignore', category=NotGeoreferencedWarning)
+
     # redirect orthority warnings to module logger
     orig_show_warning = warnings.showwarning
     warnings.showwarning = showwarning
 
     # Configure the package logger, leaving logs from dependencies on their defaults (e.g. for rasterio, they stay
     # hidden).
     # Adapted from rasterio: https://github.com/rasterio/rasterio/blob/main/rasterio/rio/main.py.
```

### Comparing `homonim-0.4.0/homonim/compare.py` & `homonim-0.4.1/homonim/compare.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/homonim/enums.py` & `homonim-0.4.1/homonim/enums.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/homonim/errors.py` & `homonim-0.4.1/homonim/errors.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/homonim/fuse.py` & `homonim-0.4.1/homonim/fuse.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/homonim/kernel_model.py` & `homonim-0.4.1/homonim/kernel_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 src_sum = cv.boxFilter(src_array, -1, kernel_shape[::-1], **filter_args)
 
             # RSS = sum((ref - ref_hat)**2)
             #     = sum((ref - (m*src + c))**2), where m and c are the first 2 bands of param_array
             # The above can be expanded and expressed in terms of cv.boxFilter kernel sums as:
             ss_res_array = (
                 ((param_array[0] ** 2) * src2_sum) +
-                (2 * np.product(param_array[:2], axis=0) * src_sum) -
+                (2 * np.prod(param_array[:2], axis=0) * src_sum) -
                 (2 * param_array[0] * src_ref_sum) -
                 (2 * param_array[1] * ref_sum) +
                 ref2_sum + (mask_sum * (param_array[1] ** 2))
             )  # yapf: disable
         else:
             # find RSS for model == Model.gain or Model.gain_blk_offset
```

### Comparing `homonim-0.4.0/homonim/matched_pair.py` & `homonim-0.4.1/homonim/matched_pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,47 +244,47 @@
         if any(src_wavelengths) and any(ref_wavelengths) and not self._force:
             # TODO: consider using a linear programming type optimisation here,
             #  e.g. https://stackoverflow.com/questions/67368093/find-optimal-unique-neighbour-pairs-based-on-closest-distance
 
             # absolute & relative distance matrix between src and ref center wavelengths
             abs_dist = np.abs(src_wavelengths[:, np.newaxis] - ref_wavelengths[np.newaxis, :])
             rel_dist = abs_dist / src_wavelengths[:, np.newaxis]
+
             def greedy_match(dist: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
                 """
                 Greedy matching of src to ref bands based on the provided center wavelength distance matrix,
                 `dist`. src bands must be down the rows, and ref bands along the cols of `dist`.
                 Will match one ref band for each src band until either all src or all ref bands
                 have been matched.  Works for all cases where len(src_bands) != len(ref_bands).
                 """
                 # match_idx[i] is the index of the ref band that matches with the ith src band
                 match_idx = np.array([np.nan] * dist.shape[0])
-                match_dist = np.array([np.nan] * dist.shape[0]) # distances corresponding to the above matches
+                match_dist = np.array([np.nan] * dist.shape[0])  # distances corresponding to the above matches
+
+                # use masked array rather than nan pass-through to avoid all-nan slice warnings
+                dist = np.ma.array(dist, mask=np.isnan(dist))
 
-                # suppress runtime warning on all-Nan slice, as it is expected in normal operation
-                with warnings.catch_warnings():
-                    warnings.simplefilter('ignore', category=RuntimeWarning)
-                    # repeat until all src or ref bands have been matched
-                    while not all(np.isnan(np.nanmin(dist, axis=1))) or not all(np.isnan(np.nanmin(dist, axis=0))):
-                        # find the row with the smallest distance in it
-                        min_dist = np.nanmin(dist, axis=1)
-                        min_dist_row_idx = np.nanargmin(min_dist)
-                        min_dist_row = dist[min_dist_row_idx, :]
-                        # store match idx and distance for this row
-                        match_idx[min_dist_row_idx] = np.nanargmin(min_dist_row)
-                        match_dist[min_dist_row_idx] = min_dist[min_dist_row_idx]
-                        # set the matched row and col to nan, so that it is not used again
-                        dist[:, int(match_idx[min_dist_row_idx])] = np.nan
-                        dist[min_dist_row_idx, :] = np.nan
+                # repeat until all src or ref bands have been matched
+                while not dist.mask.all():
+                    # find the row with the smallest distance in it
+                    min_dist = dist.min(axis=1)
+                    min_dist_row_idx = np.ma.argmin(min_dist)
+                    min_dist_row = dist[min_dist_row_idx, :]
+                    # store match idx and distance for this row
+                    match_idx[min_dist_row_idx] = np.ma.argmin(min_dist_row)
+                    match_dist[min_dist_row_idx] = min_dist[min_dist_row_idx]
+                    # set the matched row and col to nan, so that it is not used again
+                    dist[:, int(match_idx[min_dist_row_idx])] = np.ma.masked
+                    dist[min_dist_row_idx, :] = np.ma.masked
 
                 return match_dist, match_idx
 
             match_dist, match_idx = greedy_match(rel_dist)
 
-            # if any of the matched distances are greater than a threshold, raise an informative error,
-            # or log a warning, depending on `self._force`
+            # if any of the matched distances are greater than a threshold, raise an informative error
             if any(match_dist > MatchedPairReader._max_rel_wavelength_diff):
                 err_idx = match_dist > MatchedPairReader._max_rel_wavelength_diff
                 src_err_band_names = list(src_band_names[err_idx])
                 ref_err_band_names = list(ref_band_names[np.int64(match_idx[err_idx])])
                 err_dists = list(match_dist[err_idx].round(3))
                 raise ValueError(
                     f'{src_name} band(s) {src_err_band_names} could not be auto-matched.  The nearest '
```

### Comparing `homonim-0.4.0/homonim/raster_array.py` & `homonim-0.4.1/homonim/raster_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,15 +458,15 @@
             raise ImageFormatError(
                 f'The dataset resolution does not match that of the RasterArray. '
                 f'Dataset res: {rio_dataset.res}, RasterArray res: {self.res}'
             )
         if self.crs != rio_dataset.crs:
             raise ImageFormatError(
                 f'The dataset CRS does not match that of the RasterArray. '
-                f'Dataset CRS: {rio_dataset.crs.to_proj4()}, RasterArray CRS: {self.crs.to_proj4()}'
+                f'Dataset CRS: {rio_dataset.crs}, RasterArray CRS: {self.crs}'
             )
 
         if indexes is None:
             indexes = utils.get_nonalpha_bands(rio_dataset)
             indexes = indexes if len(indexes) > 1 else indexes[0]
 
         if np.any((np.array(indexes) < 1) | (np.array(indexes) > rio_dataset.count)):
@@ -474,21 +474,14 @@
             raise ValueError(f'Band index(es) {error_indexes} are out of the valid range (1..{rio_dataset.count})')
 
         if (not np.isscalar(indexes)) and (len(indexes) > self.count):
             raise ValueError(
                 f'The length of indexes ({len(indexes)}) exceeds the number of bands in the '
                 f'RasterArray ({self.count})'
             )
-        if rio_dataset.nodata is not None and (
-                self.nodata is None or not utils.nan_equals(self.nodata, rio_dataset.nodata)
-        ):
-            warnings.warn(
-                f"The dataset nodata: {rio_dataset.nodata} does not match the RasterArray nodata: {self.nodata}",
-                category=ImageFormatWarning
-            )
 
         if window is None:
             # a window defining the region in the dataset corresponding to the RasterArray extents
             window = rio_dataset.window(*self.bounds)
 
         # crop the window to dataset bounds
         window, _ = self.bounded_window_slices(rio_dataset, window)
```

### Comparing `homonim-0.4.0/homonim/raster_pair.py` & `homonim-0.4.1/homonim/raster_pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                 warnings.warn(
                     f'{name} will be re-projected to a standard North-up orientation.', category=ImageFormatWarning
                 )
 
         validate_image_format(src_im)
         validate_image_format(ref_im)
         # warn if the source and reference are not in the same CRS
-        if src_im.crs.to_proj4() != ref_im.crs.to_proj4():
+        if src_im.crs != ref_im.crs:
             src_name = Path(src_im.name).name
             ref_name = Path(ref_im.name).name
             warnings.warn(
                 f'Source and reference image will be re-projected to the same CRS: {src_name} and {ref_name}',
                 category=ImageFormatWarning
             )
 
@@ -226,16 +226,16 @@
 
     def _auto_block_shape(self, max_block_mem: float = np.inf) -> Tuple[int, int]:
         """ Find a block shape that satisfies max_block_mem. """
 
         proc_win = self._ref_win if self.proc_crs == ProcCrs.ref else self._src_win
         # adjust max_block_mem to represent the size of a block in the highest resolution image, but scaled to the
         # equivalent in proc_crs.
-        src_pix_area = np.product(np.abs(self._src_im.res))
-        ref_pix_area = np.product(np.abs(self._ref_im.res))
+        src_pix_area = np.prod(np.abs(self._src_im.res))
+        ref_pix_area = np.prod(np.abs(self._ref_im.res))
         if self.proc_crs == ProcCrs.ref:
             mem_scale = src_pix_area / ref_pix_area if ref_pix_area > src_pix_area else 1.
         elif self.proc_crs == ProcCrs.src:
             mem_scale = 1. if ref_pix_area > src_pix_area else ref_pix_area / src_pix_area
         else:
             raise ValueError("'proc_crs' has not been resolved - the raster pair must be opened first.")
         max_block_mem = max_block_mem * mem_scale if max_block_mem > 0 else np.inf
@@ -243,15 +243,15 @@
         max_block_mem *= 2 ** 20  # convert MB to bytes
         dtype_size = np.dtype(RasterArray.default_dtype).itemsize  # the size of the RasterArray data type
 
         # set the starting block_shape to correspond to the entire window
         block_shape = np.array((proc_win.height, proc_win.width)).astype('float')
 
         # keep halving the block_shape along the longest dimension until it satisfies max_block_mem
-        while (np.product(block_shape) * dtype_size) > max_block_mem:
+        while (np.prod(block_shape) * dtype_size) > max_block_mem:
             div_dim = np.argmax(block_shape)
             block_shape[div_dim] /= 2
 
         if np.any(block_shape < (1, 1)):
             raise errors.BlockSizeError(f"The auto block shape is smaller than a pixel.  Increase 'max_block_mem'.")
 
         block_shape = np.ceil(block_shape).astype('int')
```

### Comparing `homonim-0.4.0/homonim/stats.py` & `homonim-0.4.1/homonim/stats.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/homonim/utils.py` & `homonim-0.4.1/homonim/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,17 +117,17 @@
     tuple of int
         The validated kernel_shape as a numpy array.
     """
     kernel_shape = np.array(kernel_shape).astype(int)
     if not np.all(np.mod(kernel_shape, 2) == 1):
         raise ValueError('`kernel_shape` must be odd in both dimensions.')
     if model == Model.gain_offset:
-        if np.product(kernel_shape) < 2:
+        if np.prod(kernel_shape) < 2:
             raise ValueError('`kernel_shape` area should contain at least 2 elements for the gain-offset model.')
-        elif np.product(kernel_shape) < 25:
+        elif np.prod(kernel_shape) < 25:
             warnings.warn(
                 'A `kernel_shape` of at least 25 elements is recommended for the gain-offset model.',
                 category=ConfigWarning
             )
     if not np.all(kernel_shape >= 1):
         raise ValueError('`kernel_shape` must be a minimum of one in both dimensions.')
     return tuple(kernel_shape)
@@ -151,14 +151,16 @@
     # minimum of (1, 1) to avoid including extrapolated (rather than interpolated) pixels when up-sampling.
     kernel_shape = np.array(kernel_shape).astype(int)
     return tuple(np.ceil(kernel_shape / 2).astype('int'))
 
 
 def validate_threads(threads: int) -> int:
     """ Parse number of threads parameter. """
+    # TODO: Memory increases ~linearly with number of threads, but does processing speed?  The bottleneck is often
+    #  file IO & I am not sure >2 threads as a default is justified.
     _cpu_count = cpu_count()
     threads = _cpu_count if threads == 0 else threads
     if threads > _cpu_count:
         raise ValueError(f"'threads' is limited to the number of processors ({_cpu_count})")
     return threads
 
 
@@ -191,15 +193,15 @@
     """
     Re-project source and reference (as necessary) so that are they both oriented north-up, and in the same CRS.
     Re-project the proc_crs image (usually lower resolution) into the CRS of the other when the CRSs are not
     the same.
     """
     # Note: without transform etc arguments, WarpedVRT re-projects to north-up
     resampling = Resampling.bilinear
-    same_crs = src_im.crs.to_proj4() == ref_im.crs.to_proj4()
+    same_crs = src_im.crs == ref_im.crs
     if (not north_up(src_im)) and (same_crs or proc_crs != ProcCrs.src):
         src_im = WarpedVRT(src_im, crs=src_im.crs, resampling=resampling)
     if (not north_up(ref_im)) and (same_crs or proc_crs == ProcCrs.src):
         ref_im = WarpedVRT(ref_im, crs=ref_im.crs, resampling=resampling)
     if (not same_crs) and (proc_crs == ProcCrs.src):
         src_im = WarpedVRT(src_im, crs=ref_im.crs, resampling=resampling)
     if (not same_crs) and (proc_crs != ProcCrs.src):
```

### Comparing `homonim-0.4.0/homonim.egg-info/PKG-INFO` & `homonim-0.4.1/homonim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homonim
-Version: 0.4.0
+Version: 0.4.1
 Summary: Correct aerial and satellite imagery to surface reflectance.
 Author: Leftfield Geospatial
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/leftfield-geospatial/homonim
 Project-URL: Source, https://github.com/leftfield-geospatial/homonim
 Project-URL: Documentation, https://homonim.readthedocs.io
 Project-URL: Changelog, https://github.com/leftfield-geospatial/homonim/releases
@@ -34,15 +34,15 @@
 
 .. image:: https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/docs/readme_eg.webp
    :alt: example
 
 
 .. short_descr_start
 
-Correct aerial and satellite imagery to surface reflectance.
+Correct drone, aerial and satellite imagery to surface reflectance.
 
 .. short_descr_end
 .. description_start
 
 Description
 -----------
 
@@ -138,16 +138,15 @@
 .. comment
     The code below is copied from docs/examples/api_example and # [*] comments removed
 
 .. api_example_start
 
 .. code:: python
 
-    from pathlib import Path
-    from homonim import RasterFuse, RasterCompare, Model
+    from homonim import RasterFuse, Model
 
     # urls of source and reference test images
     src_file = (
         'https://raw.githubusercontent.com/leftfield-geospatial/homonim/main/'
         'tests/data/source/ngi_rgb_byte_1.tif'
     )
     ref_file = (
```

### Comparing `homonim-0.4.0/homonim.egg-info/SOURCES.txt` & `homonim-0.4.1/homonim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/pyproject.toml` & `homonim-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_compare.py` & `homonim-0.4.1/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_fuse_api.py` & `homonim-0.4.1/tests/test_fuse_api.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_fuse_cli.py` & `homonim-0.4.1/tests/test_fuse_cli.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_kernel_model.py` & `homonim-0.4.1/tests/test_kernel_model.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_matched_pair.py` & `homonim-0.4.1/tests/test_matched_pair.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     GNU Affero General Public License for more details.
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from pathlib import Path
-from typing import Tuple, List, Dict
+from typing import Tuple, List
+import warnings
 
 import numpy as np
 import pytest
 import rasterio as rio
-from rasterio import Affine
-from rasterio.windows import Window
 
 from homonim import utils
 from homonim.matched_pair import MatchedPairReader
+from homonim.errors import HomonimWarning
 
 
 @pytest.mark.parametrize(['file', 'bands', 'exp_bands', 'exp_band_names', 'exp_wavelengths'], [
     ('file_rgba', None, [1, 2, 3], ['1', '2', '3'], [.650, .560, .480]),
     ('file_rgba', (1, 2, 3), [1, 2, 3], ['1', '2', '3'], [.650, .560, .480]),
     ('file_rgba', (1, 2, 3), [1, 2, 3], ['1', '2', '3'], [.650, .560, .480]),
     ('file_masked', None, [1], ['1'], [float('nan')]),
@@ -100,17 +100,23 @@
 def test_match(
     src_file: str, ref_file: str, src_bands: Tuple, ref_bands: Tuple, exp_src_bands: List, exp_ref_bands: List,
     force: bool, request: pytest.FixtureRequest
 ):
     """ Test matching of different source and reference files. """
     src_file: Path = request.getfixturevalue(src_file)
     ref_file: Path = request.getfixturevalue(ref_file)
-    with MatchedPairReader(src_file, ref_file, src_bands=src_bands, ref_bands=ref_bands, force=force) as matched_pair:
-        assert all(np.array(matched_pair.src_bands) == exp_src_bands)
-        assert all(np.array(matched_pair.ref_bands) == exp_ref_bands)
+
+    with warnings.catch_warnings():
+        # test there are no all-nan warnings by turning them RuntimeWarning into an error, while allowing
+        # HomonimWarning which sub-classes RuntimeWarning
+        warnings.simplefilter("error", category=RuntimeWarning)
+        warnings.simplefilter("default", category=HomonimWarning)
+        with MatchedPairReader(src_file, ref_file, src_bands=src_bands, ref_bands=ref_bands, force=force) as matched_pair:
+            assert all(np.array(matched_pair.src_bands) == exp_src_bands)
+            assert all(np.array(matched_pair.ref_bands) == exp_ref_bands)
 
 
 def test_match_fewer_ref_bands_error(s2_ref_file, landsat_ref_file):
     """  Test an error is raised if num src bands > num ref bands. """
     with pytest.raises(ValueError) as ex:
         with MatchedPairReader(landsat_ref_file, s2_ref_file) as matched_pair:
             pass
```

### Comparing `homonim-0.4.0/tests/test_raster_array.py` & `homonim-0.4.1/tests/test_raster_array.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_raster_pair.py` & `homonim-0.4.1/tests/test_raster_pair.py`

 * *Files identical despite different names*

### Comparing `homonim-0.4.0/tests/test_stats.py` & `homonim-0.4.1/tests/test_stats.py`

 * *Files identical despite different names*

