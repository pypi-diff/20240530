# Comparing `tmp/subsettools-1.0.5.tar.gz` & `tmp/subsettools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsettools-1.0.5.tar", max compression
+gzip compressed data, was "subsettools-2.0.0.tar", max compression
```

## Comparing `subsettools-1.0.5.tar` & `subsettools-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-1.0.5/LICENSE
--rwxr-xr-x   0        0        0     2690 2024-05-16 18:38:12.864911 subsettools-1.0.5/README.md
--rw-r--r--   0        0        0      862 2024-05-17 15:37:58.049379 subsettools-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      612 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/__init__.py
--rw-r--r--   0        0        0      661 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_common.py
--rw-r--r--   0        0        0      154 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_constants.py
--rw-r--r--   0        0        0      820 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_dev_utils.py
--rw-r--r--   0        0        0     2928 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/_error_checking.py
--rw-r--r--   0        0        0     9261 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/clm.py
--rw-r--r--   0        0        0    19445 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/domain.py
--rw-r--r--   0        0        0    14479 2024-05-16 18:38:12.881911 subsettools-1.0.5/src/subsettools/parflow_run.py
--rw-r--r--   0        0        0    15122 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/subsetting.py
--rw-r--r--   0        0        0      147 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/__init__.py
--rw-r--r--   0        0        0    10637 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_box.yaml
--rw-r--r--   0        0        0    10190 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_solid.yaml
--rw-r--r--   0        0        0    10951 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_box.yaml
--rw-r--r--   0        0        0    10482 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_solid.yaml
--rw-r--r--   0        0        0    11495 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_box.yaml
--rw-r--r--   0        0        0    11047 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_solid.yaml
--rw-r--r--   0        0        0    11832 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_box.yaml
--rw-r--r--   0        0        0    11384 2024-05-16 18:38:12.882911 subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_solid.yaml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 subsettools-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1092 2023-11-13 19:24:51.323232 subsettools-2.0.0/LICENSE
+-rwxr-xr-x   0        0        0     2690 2024-05-16 18:38:12.864911 subsettools-2.0.0/README.md
+-rw-r--r--   0        0        0      862 2024-05-30 18:16:46.450912 subsettools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      612 2024-05-16 18:38:12.881911 subsettools-2.0.0/src/subsettools/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-24 03:38:00.649713 subsettools-2.0.0/src/subsettools/_common.py
+-rw-r--r--   0        0        0      154 2024-05-16 18:38:12.881911 subsettools-2.0.0/src/subsettools/_constants.py
+-rw-r--r--   0        0        0      820 2024-05-16 18:38:12.881911 subsettools-2.0.0/src/subsettools/_dev_utils.py
+-rw-r--r--   0        0        0     2928 2024-05-16 18:38:12.881911 subsettools-2.0.0/src/subsettools/_error_checking.py
+-rw-r--r--   0        0        0     9092 2024-05-30 18:07:55.783453 subsettools-2.0.0/src/subsettools/clm.py
+-rw-r--r--   0        0        0    19074 2024-05-30 17:55:14.853972 subsettools-2.0.0/src/subsettools/domain.py
+-rw-r--r--   0        0        0    14479 2024-05-16 18:38:12.881911 subsettools-2.0.0/src/subsettools/parflow_run.py
+-rw-r--r--   0        0        0    15449 2024-05-25 22:46:50.416538 subsettools-2.0.0/src/subsettools/subsetting.py
+-rw-r--r--   0        0        0      147 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/__init__.py
+-rw-r--r--   0        0        0    10637 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus1_spinup_box.yaml
+-rw-r--r--   0        0        0    10190 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus1_spinup_solid.yaml
+-rw-r--r--   0        0        0    10951 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus1_transient_box.yaml
+-rw-r--r--   0        0        0    10482 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus1_transient_solid.yaml
+-rw-r--r--   0        0        0    11495 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus2_spinup_box.yaml
+-rw-r--r--   0        0        0    11047 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus2_spinup_solid.yaml
+-rw-r--r--   0        0        0    11832 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus2_transient_box.yaml
+-rw-r--r--   0        0        0    11384 2024-05-16 18:38:12.882911 subsettools-2.0.0/src/subsettools/template_runscripts/conus2_transient_solid.yaml
+-rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 subsettools-2.0.0/PKG-INFO
```

### Comparing `subsettools-1.0.5/LICENSE` & `subsettools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/README.md` & `subsettools-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/pyproject.toml` & `subsettools-2.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subsettools"
-version = "1.0.5"
+version = "2.0.0"
 description = "Subsetting tools and utilities for ParFlow"
 authors = ["George Artavanis, Amanda Triplett"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `subsettools-1.0.5/src/subsettools/__init__.py` & `subsettools-2.0.0/src/subsettools/__init__.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/_dev_utils.py` & `subsettools-2.0.0/src/subsettools/_dev_utils.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/_error_checking.py` & `subsettools-2.0.0/src/subsettools/_error_checking.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/clm.py` & `subsettools-2.0.0/src/subsettools/clm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 from datetime import timedelta
 import numpy as np
 import hf_hydrodata
 from ._common import (
     get_utc_time,
+    get_hf_gridded_data,
 )
 from ._error_checking import (
     _validate_dir,
     _validate_grid_bounds,
     _validate_date,
 )
 
@@ -81,29 +82,26 @@
                 )
             except ValueError as err:
                 print(f"Failed to get {file_type} file for dataset '{dataset}':", err)
             else:
                 file_paths[file_type] = file_path
                 print("copied vegp")
         elif file_type == "pfb":
-            try:
-                subset_data = hf_hydrodata.get_gridded_data(
-                    dataset=dataset,
-                    file_type=file_type,
-                    variable="clm_run",
-                    temporal_resolution="static",
-                    grid_bounds=ij_bounds,
-                )
-            except ValueError as err:
-                print(f"Failed to get vegm file for dataset '{dataset}':", err)
-            else:
-                land_cover_data = _reshape_ndarray_to_vegm_format(subset_data)
-                file_path = _write_land_cover(land_cover_data, write_dir)
-                file_paths[file_type] = file_path
-                print("subset vegm")
+            options = {
+                "dataset": dataset,
+                "file_type": file_type,
+                "variable": "clm_run",
+                "temporal_resolution": "static",
+                "grid_bounds": ij_bounds,
+            }
+            subset_data = get_hf_gridded_data(options)
+            land_cover_data = _reshape_ndarray_to_vegm_format(subset_data)
+            file_path = _write_land_cover(land_cover_data, write_dir)
+            file_paths[file_type] = file_path
+            print("subset vegm")
         elif file_type == "drv_clm":
             file_path = os.path.join(write_dir, "drv_clmin.dat")
             try:
                 hf_hydrodata.get_raw_file(
                     file_path,
                     dataset=dataset,
                     file_type=file_type,
@@ -227,23 +225,21 @@
     assert (start is None and end is None) or (start is not None and end is not None)
 
     with open(file_path, encoding="utf-8") as f:
         lines = f.readlines()
 
     for i, line in enumerate(lines):
         if "vegtf" in line:
-            lines[i] = (
-                f"{'vegtf':<15}{vegm_name:<37} Vegetation Tile Specification File\n"
-            )
+            lines[
+                i
+            ] = f"{'vegtf':<15}{vegm_name:<37} Vegetation Tile Specification File\n"
         elif "vegpf" in line:
             lines[i] = f"{'vegpf':<15}{vegp_name:<37} Vegetation Type Parameter\n"
         elif "startcode" in line:
-            lines[i] = (
-                f"{'startcode':<15}{startcode:<37} 1=restart file, 2=defined\n"
-            )
+            lines[i] = f"{'startcode':<15}{startcode:<37} 1=restart file, 2=defined\n"
         elif "clm_ic" in line:
             lines[i] = f"{'clm_ic':<15}{startcode:<37} 1=restart file, 2=defined\n"
 
     if start is not None:
         start_date = get_utc_time(start, time_zone)
         end_date = get_utc_time(end, time_zone) - timedelta(hours=1)
```

### Comparing `subsettools-1.0.5/src/subsettools/domain.py` & `subsettools-2.0.0/src/subsettools/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from ._error_checking import (
     _validate_huc_list,
     _validate_grid,
     _validate_latlon_list,
     _validate_dir,
     _validate_mask,
 )
+from ._common import (
+    get_hf_gridded_data,
+)
 from ._constants import (
     CONUS_DX,
     CONUS_DY,
     CONUS1_DZ,
     CONUS1_Z_TOP,
     CONUS2_DZ,
     CONUS2_Z_TOP,
@@ -83,25 +86,21 @@
         )
     """
     _validate_huc_list(hucs)
     _validate_grid(grid)
 
     huc_len = len(hucs[0])
     hucs = [int(huc) for huc in hucs]
-    try:
-        conus_hucs = hf_hydrodata.get_gridded_data(
-            dataset="huc_mapping",
-            grid=grid,
-            file_type="tiff",
-            level=str(huc_len),
-        )
-    except Exception as exc:
-        raise ValueError(
-            f"Failed to get huc mapping data for the grid {grid}."
-        ) from exc
+    options = {
+        "dataset": "huc_mapping",
+        "grid": grid,
+        "file_type": "tiff",
+        "level": str(huc_len),
+    }
+    conus_hucs = get_hf_gridded_data(options)
     huc_mask = np.isin(conus_hucs, hucs).squeeze()
     indices_j, indices_i = np.where(huc_mask > 0)
     if indices_i.size == 0 or indices_j.size == 0:
         raise ValueError(
             f"The area defined by the provided HUCs is not part of the {grid} grid."
         )
 
@@ -221,25 +220,21 @@
     point0, point1 = [
         hf_hydrodata.to_ij(grid, latlon_pt[0], latlon_pt[1])
         for latlon_pt in latlon_bounds
     ]
     imin, imax = [min(point0[0], point1[0]), max(point0[0], point1[0]) + 1]
     jmin, jmax = [min(point0[1], point1[1]), max(point0[1], point1[1]) + 1]
     grid_bounds = (imin, jmin, imax, jmax)
-    try:
-        mask = hf_hydrodata.get_gridded_data(
-            dataset="huc_mapping",
-            grid=grid,
-            level="2",
-            grid_bounds=grid_bounds,
-        )
-    except Exception as exc:
-        raise ValueError(
-            f"Failed to get huc mapping data for the grid {grid}."
-        ) from exc
+    options = {
+        "dataset": "huc_mapping",
+        "grid": grid,
+        "level": "2",
+        "grid_bounds": grid_bounds,
+    }
+    mask = get_hf_gridded_data(options)
     mask[mask > 0] = 1
     return grid_bounds, mask.astype(int)
 
 
 def latlon_to_ij(latlon_bounds, grid):
     """This function is deprecated.
 
@@ -493,22 +488,20 @@
             outlets=[[44.1348, -95.5084], [44.1352, -95.4949]],
             grid="conus2"
         )
     """
     _validate_latlon_list(outlets)
     _validate_grid(grid)
     grid = grid.lower()
-    try:
-        flow_direction = hf_hydrodata.get_gridded_data(
-            variable="flow_direction", grid=grid, file_type="tiff"
-        )
-    except Exception as exc:
-        raise ValueError(
-            f"Failed to get flow direction data for the grid {grid}."
-        ) from exc
+    options = {
+        "variable": "flow_direction",
+        "grid": grid,
+        "file_type": "tiff",
+    }
+    flow_direction = get_hf_gridded_data(options)
     nj, ni = flow_direction.shape
     marked = np.zeros((nj, ni), dtype=int)
     flow_values = [1, 2, 3, 4]  # D4 neighbors
     directions = np.array([[0, -1], [-1, 0], [0, 1], [1, 0]])
     queue = [hf_hydrodata.to_ij(grid, outlet[0], outlet[1]) for outlet in outlets]
 
     for point in queue:
```

### Comparing `subsettools-1.0.5/src/subsettools/parflow_run.py` & `subsettools-2.0.0/src/subsettools/parflow_run.py`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/subsetting.py` & `subsettools-2.0.0/src/subsettools/subsetting.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     - subset gridded CLM inputs (vegm)
 """
 
 import os
 from datetime import datetime, timedelta
 import threading
 import re
+import warnings
 import numpy as np
 import hf_hydrodata
 from parflow.tools.io import write_pfb
 from ._common import (
     get_utc_time,
+    get_hf_gridded_data,
 )
 from ._error_checking import (
     _validate_grid,
     _validate_dir,
     _validate_grid_bounds,
     _validate_date,
 )
@@ -48,74 +50,93 @@
     The subset values will be written as ParFlow binary files (pfbs) in
     write_dir. By default the following variables will be subset.
         - Slope in the east/west direction (slope_x)
         - Slope in the north/south direction (slope_y)
         - Subsurface units indicator file (pf_indicator)
         - Mannings roughness coefficients (mannings)
         - Depth to bedrock (pf_flowbarrier)
-        - Long term average preciptation minus evaporation (i.e. recharge) (pme)
+        - Long term average precipitation minus evaporation (i.e. recharge) (pme)
         - Steady state pressure head used to initialize transient simulations
           (ss_pressure_head)
 
     Note that some datasets might not contain all 7 static input variables. In
-    that case, the subset_static function is going to get and save the data for
-    the variables supported by the dataset and print out a message for those
-    that are not.
+    that case, the subset_static function is going to raise a ValueError for any
+    variables that do not exist in the dataset. The default variable list
+    contains the necessary static variables for the CONUS2 grid. For CONUS1-based
+    datasets, "mannings" and "pf_flowbarrier" should be removed from the list.
 
     Args:
         ij_bounds (tuple[int]): bounding box for subset. This should be given as
             i,j index values where 0,0 is the lower left hand corner of a domain.
             ij_bounds are given relative to whatever grid is being used for the
             subset.
         dataset (str): static inputs dataset name from the HydroData catalog e.g.
             "conus1_domain"
         write_dir (str): directory where the subset files will be written
         var_list (tuple[str]): tuple of variables to subset from the dataset.
             By default all 7 variables above will be subset. The user can specify
-            as subset of these variables or list additional variables that are
+            a subset of these variables or list additional variables that are
             available in their dataset of choice.
 
     Returns:
         A dictionary mapping the static variable names to the corresponding file
         paths where the subset data were written.
 
     Example:
 
     .. code-block:: python
 
+        # Subsetting static variables for a CONUS1 workflow
+        # We need to remove "pf_flowbarrier" and "mannings" from the list
         filepaths = subset_static(
             ij_bounds=(375, 239, 487, 329),
             dataset="conus1_domain",
             write_dir="/path/to/your/chosen/directory",
-            var_list=("slope_x", "slope_y")
+            var_list=("slope_x", "slope_y", "pf_indicator", "pme",
+                      "ss_pressure_head")
+        )
+
+        # Subsetting static variables for a CONUS2 workflow
+        # Note that we can use the default var_list here
+        filepaths = subset_static(
+            ij_bounds=(3701, 1544, 3792, 1633),
+            dataset="conus2_domain",
+            write_dir="/path/to/your/chosen/directory",
         )
     """
+    warnings.warn(
+        "Note that for subsettools versions >= 2.0.0, this function will raise "
+        "a ValueError if a variable in var_list is not supported in the "
+        "dataset. (In older versions, it just printed an error message and "
+        "continued executing normally). You can check in the HydroData "
+        "documentation which variables are contained in each dataset "
+        "(https://hf-hydrodata.readthedocs.io/en/latest/available_data.html).",
+        DeprecationWarning,
+        stacklevel=2,
+    )
     _validate_grid_bounds(ij_bounds)
     if not isinstance(dataset, str):
         raise TypeError("dataset name must be a string.")
     _validate_dir(write_dir)
     if not all(isinstance(var, str) for var in var_list):
         raise TypeError("All variable names should be strings.")
     file_paths = {}
+    options = {
+        "dataset": dataset,
+        "file_type": "pfb",
+        "temporal_resolution": "static",
+        "grid_bounds": ij_bounds,
+    }
     for var in var_list:
-        try:
-            subset_data = hf_hydrodata.get_gridded_data(
-                dataset=dataset,
-                variable=var,
-                file_type="pfb",
-                temporal_resolution="static",
-                grid_bounds=ij_bounds,
-            )
-        except ValueError as err:
-            print(f"Variable '{var}' not found in dataset '{dataset}':", err)
-        else:
-            file_path = os.path.join(write_dir, f"{var}.pfb")
-            write_pfb(file_path, subset_data, dist=False)
-            file_paths[var] = file_path
-            print(f"Wrote {var}.pfb in specified directory.")
+        options["variable"] = var
+        subset_data = get_hf_gridded_data(options)
+        file_path = os.path.join(write_dir, f"{var}.pfb")
+        write_pfb(file_path, subset_data, dist=False)
+        file_paths[var] = file_path
+        print(f"Wrote {var}.pfb in specified directory.")
 
     return file_paths
 
 
 def subset_press_init(ij_bounds, dataset, date, write_dir, time_zone="UTC"):
     """Subset a pressure file from a national dataset in HydroData.
 
@@ -161,27 +182,23 @@
     if not isinstance(time_zone, str):
         raise TypeError("time_zone must be a string.")
 
     new_date = get_utc_time(date, time_zone)
     print(f"UTC Date: {new_date}")
     date_string = new_date.strftime("%Y.%m.%d:%H.%M.%S_UTC0")
 
-    try:
-        subset_data = hf_hydrodata.get_gridded_data(
-            dataset=dataset,
-            variable="pressure_head",
-            file_type="pfb",
-            temporal_resolution="hourly",
-            grid_bounds=ij_bounds,
-            start_time=new_date,
-        )
-    except ValueError as err:
-        print(f"No pressure file found in dataset '{dataset}':", err)
-        return None
-
+    options = {
+        "dataset": dataset,
+        "variable": "pressure_head",
+        "file_type": "pfb",
+        "temporal_resolution": "hourly",
+        "grid_bounds": ij_bounds,
+        "start_time": new_date,
+    }
+    subset_data = get_hf_gridded_data(options)
     file_path = os.path.join(write_dir, f"{dataset}_{date_string}_press.pfb")
     write_pfb(file_path, subset_data[0, :, :, :], dist=False)
     print(f"Wrote {file_path} in specified directory.")
     return file_path
 
 
 def subset_forcing(
@@ -258,141 +275,123 @@
     if not isinstance(dataset, str):
         raise TypeError("dataset name must be a string.")
     _validate_dir(write_dir)
     if not isinstance(time_zone, str):
         raise TypeError("time_zone must be a string.")
     if not all(isinstance(var, str) for var in forcing_vars):
         raise TypeError("All variable names should be strings.")
+    forcing_vars = tuple(set(forcing_vars))
     outputs = {}
     start_date = get_utc_time(start, time_zone)
     end_date = get_utc_time(end, time_zone)
     exit_event = threading.Event()
+    lock = threading.Lock()
     threads = [
         threading.Thread(
             target=_subset_forcing_variable,
             args=(
                 variable,
                 ij_bounds,
                 grid,
                 start_date,
                 end_date,
                 dataset,
                 write_dir,
                 time_zone,
                 outputs,
                 exit_event,
+                lock,
             ),
         )
         for variable in forcing_vars
     ]
 
     for thread in threads:
         thread.start()
 
     try:
         for thread in threads:
             thread.join()
     except KeyboardInterrupt:
         print("Interrupted. Stopping threads...")
         exit_event.set()
-
         for thread in threads:
             thread.join()
-
         print("All threads stopped.")
-    finally:
-        return outputs
+
+    if exit_event.is_set():
+        raise ValueError("One or more threads were interrupted.")
+    return outputs
 
 
 def _subset_forcing_variable(
     variable,
     ij_bounds,
     grid,
     start_date,
     end_date,
     dataset,
     write_dir,
     time_zone,
     outputs,
     exit_event,
+    lock,
 ):
     """Helper for subset_forcing that subsets data for one forcing variable."""
 
     day = 1
     date = start_date
     delta = timedelta(hours=_HOURS_PER_FORCING_FILE)
-    outputs[variable] = []
+    write_paths = []
     print(f"Reading {variable} pfb sequence")
+    options = {
+        "dataset": dataset,
+        "variable": variable,
+        "grid": grid,
+        "file_type": "pfb",
+        "temporal_resolution": "hourly",
+        "grid_bounds": ij_bounds,
+    }
 
     while date < end_date and not exit_event.is_set():
         start_time = date
         end_time = date + delta
         # we need to distinguish between UTC and non-UTC as the datacatalog
         # returns the wrong answer for requests that start reading from the
         # middle of a file and span multiple files
         try:
             if time_zone == "UTC":
-                subset_data = hf_hydrodata.get_gridded_data(
-                    dataset=dataset,
-                    variable=variable,
-                    grid=grid,
-                    file_type="pfb",
-                    temporal_resolution="hourly",
-                    start_time=start_time,
-                    end_time=end_time,
-                    grid_bounds=ij_bounds,
-                )
+                options["start_time"] = start_time
+                options["end_time"] = end_time
+                subset_data = get_hf_gridded_data(options)
             else:
                 next_day_midnight = datetime(
                     end_time.year, end_time.month, end_time.day
                 )
-                data1 = hf_hydrodata.get_gridded_data(
-                    dataset=dataset,
-                    variable=variable,
-                    grid=grid,
-                    file_type="pfb",
-                    temporal_resolution="hourly",
-                    start_time=start_time,
-                    end_time=next_day_midnight,
-                    grid_bounds=ij_bounds,
-                )
-                data2 = hf_hydrodata.get_gridded_data(
-                    dataset=dataset,
-                    variable=variable,
-                    grid=grid,
-                    file_type="pfb",
-                    temporal_resolution="hourly",
-                    start_time=next_day_midnight,
-                    end_time=end_time,
-                    grid_bounds=ij_bounds,
-                )
-                subset_data = np.concatenate((data1, data2), axis=0)
-        except Exception as exc:
-            raise ValueError(
-                f"Failed to get {variable} data from {start_time} to {end_time}."
-            ) from exc
-
-        paths = hf_hydrodata.get_paths(
-            dataset=dataset,
-            variable=variable,
-            grid=grid,
-            file_type="pfb",
-            temporal_resolution="hourly",
-            start_time=start_time,
-            end_time=end_time,
-        )
-
+                options["start_time"] = start_time
+                options["end_time"] = next_day_midnight
+                data_day1 = get_hf_gridded_data(options)
+                options["start_time"] = next_day_midnight
+                options["end_time"] = end_time
+                data_day2 = get_hf_gridded_data(options)
+                subset_data = np.concatenate((data_day1, data_day2), axis=0)
+        except Exception:
+            exit_event.set()
+            raise
+        paths = hf_hydrodata.get_paths(options)
         write_path = os.path.join(
             write_dir, _adjust_filename_hours(os.path.basename(paths[0]), day)
         )
-        outputs[variable].append(write_path)
+        write_paths.append(write_path)
         write_pfb(write_path, subset_data[:, :, :], dist=False)
         date = date + delta
         day = day + 1
     if not exit_event.is_set():
+        with lock:
+            outputs[variable] = write_paths
         print(f"Finished writing {variable} to folder")
 
 
 def _adjust_filename_hours(filename, day):
     """Adjust the part of the the forcing filename representing hours.
 
     The aim is to match what a parflow simulation expects on each day of the
```

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_box.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus1_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_spinup_solid.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus1_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_box.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus1_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus1_transient_solid.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus1_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_box.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus2_spinup_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_spinup_solid.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus2_spinup_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_box.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus2_transient_box.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/src/subsettools/template_runscripts/conus2_transient_solid.yaml` & `subsettools-2.0.0/src/subsettools/template_runscripts/conus2_transient_solid.yaml`

 * *Files identical despite different names*

### Comparing `subsettools-1.0.5/PKG-INFO` & `subsettools-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subsettools
-Version: 1.0.5
+Version: 2.0.0
 Summary: Subsetting tools and utilities for ParFlow
 License: MIT
 Author: George Artavanis, Amanda Triplett
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

