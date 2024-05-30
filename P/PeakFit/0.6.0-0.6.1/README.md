# Comparing `tmp/peakfit-0.6.0.tar.gz` & `tmp/peakfit-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakfit-0.6.0.tar", last modified: Tue May 28 20:20:43 2024, max compression
+gzip compressed data, was "peakfit-0.6.1.tar", last modified: Thu May 30 12:54:24 2024, max compression
```

## Comparing `peakfit-0.6.0.tar` & `peakfit-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34916 2024-05-28 20:20:31.933946 peakfit-0.6.0/LICENSE
--rw-r--r--   0        0        0       75 2024-05-28 20:20:31.933946 peakfit-0.6.0/README.md
--rw-r--r--   0        0        0       73 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/__init__.py
--rw-r--r--   0        0        0      126 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/__main__.py
--rw-r--r--   0        0        0     1431 2024-05-28 20:20:32.345948 peakfit-0.6.0/peakfit/cli.py
--rw-r--r--   0        0        0     3903 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/clustering.py
--rw-r--r--   0        0        0     1243 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/computing.py
--rw-r--r--   0        0        0     2602 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/messages.py
--rw-r--r--   0        0        0      467 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/noise.py
--rw-r--r--   0        0        0     8970 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/peakfit.py
--rw-r--r--   0        0        0     3175 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/peaklist.py
--rw-r--r--   0        0        0     1678 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_cest.py
--rw-r--r--   0        0        0     2725 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_cpmg.py
--rw-r--r--   0        0        0     1225 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plot_intensities.py
--rw-r--r--   0        0        0     2900 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/plots.py
--rw-r--r--   0        0        0     2039 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/shapes.py
--rw-r--r--   0        0        0        0 2024-05-28 20:20:32.349948 peakfit-0.6.0/peakfit/writing.py
--rw-r--r--   0        0        0     1203 2024-05-28 20:20:43.769992 peakfit-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 peakfit-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-30 12:54:18.392443 peakfit-0.6.1/LICENSE
+-rw-r--r--   0        0        0       75 2024-05-30 12:54:18.392443 peakfit-0.6.1/README.md
+-rw-r--r--   0        0        0       73 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/__init__.py
+-rw-r--r--   0        0        0      126 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/__main__.py
+-rw-r--r--   0        0        0     1545 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/cli.py
+-rw-r--r--   0        0        0     4103 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/clustering.py
+-rw-r--r--   0        0        0     1243 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/computing.py
+-rw-r--r--   0        0        0     2602 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/messages.py
+-rw-r--r--   0        0        0      467 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/noise.py
+-rw-r--r--   0        0        0     9019 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/peakfit.py
+-rw-r--r--   0        0        0     3304 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/peaklist.py
+-rw-r--r--   0        0        0     1678 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/plot_cest.py
+-rw-r--r--   0        0        0     2725 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/plot_cpmg.py
+-rw-r--r--   0        0        0     1225 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/plot_intensities.py
+-rw-r--r--   0        0        0     3192 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/plots.py
+-rw-r--r--   0        0        0     2039 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/shapes.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:54:18.808446 peakfit-0.6.1/peakfit/writing.py
+-rw-r--r--   0        0        0     1203 2024-05-30 12:54:24.344479 peakfit-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 peakfit-0.6.1/PKG-INFO
```

### Comparing `peakfit-0.6.0/LICENSE` & `peakfit-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/cli.py` & `peakfit-0.6.1/peakfit/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,9 +36,12 @@
         nargs=5,
         metavar=("X_MIN", "X_MAX", "Y_MIN", "Y_MAX", "N"),
     )
     parser.add_argument("--fixed", dest="fixed", action="store_true")
     parser.add_argument("--pvoigt", dest="pvoigt", action="store_true")
     parser.add_argument("--lorentzian", dest="lorentzian", action="store_true")
     parser.add_argument("--exclude", dest="exclude", type=int, nargs="+")
+    parser.add_argument(
+        "--merge-cluster-threshold", dest="merge_cluster_threshold_hz", type=float
+    )
 
     return parser
```

### Comparing `peakfit-0.6.0/peakfit/clustering.py` & `peakfit-0.6.1/peakfit/clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import product
 from typing import NamedTuple
 
 import numpy as np
 import pandas as pd
 from nmrglue.fileio.fileiobase import unit_conversion
 from scipy import spatial
+from scipy.cluster.hierarchy import fcluster, single
 
 from peakfit.messages import print_segmenting
 
 
 class Spectra(NamedTuple):
     data: np.ndarray
     ucx: unit_conversion
@@ -20,64 +21,66 @@
 class Cluster(NamedTuple):
     peaks: pd.DataFrame
     x: np.ndarray
     y: np.ndarray
     data: np.ndarray
 
 
-def _merge_clusters(cluster1: Cluster, cluster2: Cluster) -> Cluster:
-    cluster_peaks = pd.concat([cluster1.peaks, cluster2.peaks]).reset_index(drop=True)
-    cluster_x = np.hstack((cluster1.x, cluster2.x))
-    cluster_y = np.hstack((cluster1.y, cluster2.y))
-    cluster_data = np.vstack((cluster1.data, cluster2.data))
+def _merge_clusters(clusters: list[Cluster]) -> Cluster:
+    cluster_peaks = pd.concat([cluster.peaks for cluster in clusters]).reset_index(
+        drop=True
+    )
+    cluster_x = np.hstack([cluster.x for cluster in clusters])
+    cluster_y = np.hstack([cluster.y for cluster in clusters])
+    cluster_data = np.vstack([cluster.data for cluster in clusters])
     return Cluster(cluster_peaks, cluster_x, cluster_y, cluster_data)
 
 
 def _distance(cluster1: Cluster, cluster2: Cluster) -> float:
     points1 = cluster1.peaks[["x0_hz", "y0_hz"]]
     points2 = cluster2.peaks[["x0_hz", "y0_hz"]]
     distances = spatial.distance.cdist(points1, points2)
     return np.min(distances)
 
 
-def _merge_close_clusters(
+def _merge_close_clusters2(
     clusters: list[Cluster],
     cutoff: float,
 ) -> list[Cluster]:
-    grouped = True
-    while grouped:
-        grouped = False
-        for cluster1, cluster2 in it.combinations(clusters, 2):
-            if _distance(cluster1, cluster2) <= cutoff:
-                merged = _merge_clusters(cluster1, cluster2)
-                clusters.remove(cluster1)
-                clusters.remove(cluster2)
-                clusters.append(merged)
-                grouped = True
-                break
-    return clusters
+    pdist = np.array(
+        [
+            _distance(cluster1, cluster2)
+            for cluster1, cluster2 in it.combinations(clusters, 2)
+        ]
+    )
+    dendrogram = single(pdist)
+    clusters_ids = fcluster(dendrogram, t=cutoff, criterion="distance")
+
+    if len(clusters) == len(np.unique(clusters_ids)):
+        return clusters
+
+    clusters_dict: dict[int, list[Cluster]] = {}
+    for i, cluster in zip(clusters_ids, clusters, strict=False):
+        clusters_dict.setdefault(i, []).append(cluster)
+
+    return [_merge_clusters(cluster_list) for cluster_list in clusters_dict.values()]
 
 
 def _select_square(x: int, y: int, size: int) -> set[tuple[int, int]]:
     size = size // 2
     return set(product(range(x - size, x + size + 1), range(y - size, y + size + 1)))
 
 
 def _flood(
     x_start: int,
     y_start: int,
     spectra: Spectra,
     threshold: float,
 ) -> pd.DataFrame:
     data = spectra.data
-    # peaks = ng.peakpick.pick(data[0], pthres=threshold, nthres=-threshold)
-    # print(peaks)
-    # print(peaks.dtype.names)
-    # print(Counter(peaks.cID))
-    # sys.exit()
     data_above = np.any(np.absolute(data) >= threshold, axis=0)
     _nz, ny, nx = data.shape
     stack = [(x_start, y_start)]
     points: set[tuple[int, int]] = set()
     while stack:
         x, y = stack.pop()
         x %= nx
@@ -99,14 +102,15 @@
     return region_data.reshape((nz, len(region))).T
 
 
 def cluster_peaks(
     spectra: Spectra,
     peaks: pd.DataFrame,
     contour_level: float,
+    merge_cluster_threshold_hz: float | None = None,
 ) -> list[Cluster]:
     print_segmenting()
 
     clusters = []
     selected_peaks: set[str] = set()
 
     for peak in peaks.itertuples(index=False, name="Peak"):
@@ -117,10 +121,11 @@
         cluster_x = region["x0_int"].to_numpy()
         cluster_y = region["y0_int"].to_numpy()
         cluster_data = get_cluster_data(spectra.data, region)
         cluster = Cluster(cluster_peaks, cluster_x, cluster_y, cluster_data)
         clusters.append(cluster)
         selected_peaks = {*selected_peaks, *cluster_peaks["name"]}
 
-    clusters = _merge_close_clusters(clusters, 20.0)
+    if merge_cluster_threshold_hz is not None:
+        clusters = _merge_close_clusters2(clusters, merge_cluster_threshold_hz)
 
     return sorted(clusters, key=lambda x: len(x[0]))
```

### Comparing `peakfit-0.6.0/peakfit/computing.py` & `peakfit-0.6.1/peakfit/computing.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/messages.py` & `peakfit-0.6.1/peakfit/messages.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/peakfit.py` & `peakfit-0.6.1/peakfit/peakfit.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,17 @@
 
     peaks = read_list(clargs.path_list, spectra)
     clargs.path_output.mkdir(parents=True, exist_ok=True)
 
     if clargs.contour_level is None:
         clargs.contour_level = 5.0 * clargs.noise
 
-    clusters = cluster_peaks(spectra, peaks, clargs.contour_level)
+    clusters = cluster_peaks(
+        spectra, peaks, clargs.contour_level, clargs.merge_cluster_threshold_hz
+    )
     shifts = run_fit(clargs, spectra, clusters)
 
     export_html(clargs.path_output / "logs.html")
     write_shifts(peaks["name"], shifts, clargs.path_output / "shifts.list")
 
 
 if __name__ == "__main__":
```

### Comparing `peakfit-0.6.0/peakfit/peaklist.py` & `peakfit-0.6.1/peakfit/peaklist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Callable, Iterable
+from io import StringIO
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 from peakfit.clustering import Spectra
 
@@ -33,16 +34,18 @@
     peaks["y0_hz"] = spectra.ucy.hz(peaks["y0_pt"])
     return peaks
 
 
 @register_reader("list")
 def read_sparky_list(path: Path, spectra: Spectra) -> pd.DataFrame:
     """Read a Sparky list file and return a list of peaks."""
+    with path.open() as f:
+        text = "\n".join([line for line in f if "Ass" not in line])
     peaks = pd.read_table(
-        path,
+        StringIO(text),
         sep=r"\s+",
         comment="#",
         header=None,
         encoding="utf-8",
         names=("name", "y0_ppm", "x0_ppm"),
     )
     return _complete_peak_infos(peaks, spectra)
```

### Comparing `peakfit-0.6.0/peakfit/plot_cest.py` & `peakfit-0.6.1/peakfit/plot_cest.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/plot_cpmg.py` & `peakfit-0.6.1/peakfit/plot_cpmg.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/plot_intensities.py` & `peakfit-0.6.1/peakfit/plot_intensities.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/peakfit/plots.py` & `peakfit-0.6.1/peakfit/plots.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     contour_level (float): The starting contour level.
     out (MinimizerResult): The result from the minimizer containing fit parameters.
     """
     # Calculate contour levels
     cl = contour_level * CONTOUR_FACTOR ** np.arange(CONTOUR_NUM)
     cl = np.concatenate((-cl[::-1], cl))
 
-    data = spectra.data[0]
+    # Find the spectrum with the more signal
+    plane_index = np.linalg.norm(spectra.data[:, cluster.y, cluster.x], axis=1).argmax()
+
+    data = spectra.data[plane_index]
     cluster_data = np.zeros_like(data)
     cluster_calc = np.zeros_like(data)
 
     nz, ny, nx = spectra.data.shape
 
     min_x, max_x = np.min(cluster.x), np.max(cluster.x)
     min_y, max_y = np.min(cluster.y), np.max(cluster.y)
@@ -78,14 +81,21 @@
         0.05,
         0.95,
         f"{chi2red_str} {out.redchi:.2f}",
         transform=ax.transAxes,
         verticalalignment="top",
         bbox=CHI2_BOX_PROPS,
     )
+    ax.text(
+        0.85,
+        0.05,
+        f"Plane: {plane_index}\n",
+        transform=ax.transAxes,
+        verticalalignment="top",
+    )
 
     # Decorate the axes
     ax.set_ylabel("F1 (pt)")
     ax.set_xlabel("F2 (pt)")
     ax.set_title(", ".join(peaks["name"]))
     ax.set_xlim(min_x, max_x)
     ax.set_ylim(min_y, max_y)
```

### Comparing `peakfit-0.6.0/peakfit/shapes.py` & `peakfit-0.6.1/peakfit/shapes.py`

 * *Files identical despite different names*

### Comparing `peakfit-0.6.0/pyproject.toml` & `peakfit-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "pandas>=2.2.2",
     "scipy>=1.13.1",
     "openpyxl>=3.1.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dynamic = []
-version = "0.6.0"
+version = "0.6.1"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.scripts]
 peakfit = "peakfit.peakfit:main"
 plot_cpmg = "peakfit.plot_cpmg:main"
```

### Comparing `peakfit-0.6.0/PKG-INFO` & `peakfit-0.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PeakFit
-Version: 0.6.0
+Version: 0.6.1
 Summary: PeakFit allow for lineshape fitting in pseudo-3D NMR spectra.
 Author-Email: Guillaume Bouvignies <guillaume.bouvignies@ens.psl.eu>
 License: GPL-3.0-or-later
 Requires-Python: >=3.11
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: lmfit>=1.3.1
 Requires-Dist: matplotlib>=3.9.0
```

