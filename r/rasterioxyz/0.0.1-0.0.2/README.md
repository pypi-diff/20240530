# Comparing `tmp/rasterioxyz-0.0.1.tar.gz` & `tmp/rasterioxyz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterioxyz-0.0.1.tar", max compression
+gzip compressed data, was "rasterioxyz-0.0.2.tar", max compression
```

## Comparing `rasterioxyz-0.0.1.tar` & `rasterioxyz-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-02-02 17:31:52.640287 rasterioxyz-0.0.1/LICENSE
--rw-r--r--   0        0        0    10547 2024-02-02 17:31:52.640287 rasterioxyz-0.0.1/README.md
--rw-r--r--   0        0        0      639 2024-02-02 17:31:52.644286 rasterioxyz-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-02 17:31:52.644286 rasterioxyz-0.0.1/rasterioxyz/__init__.py
--rw-r--r--   0        0        0       68 2024-02-02 17:31:52.644286 rasterioxyz-0.0.1/rasterioxyz/_errors.py
--rw-r--r--   0        0        0     1118 2024-02-02 17:31:52.644286 rasterioxyz-0.0.1/rasterioxyz/_utils.py
--rw-r--r--   0        0        0    17546 2024-02-02 17:31:52.644286 rasterioxyz-0.0.1/rasterioxyz/tile.py
--rw-r--r--   0        0        0    11165 1970-01-01 00:00:00.000000 rasterioxyz-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-30 15:39:19.266956 rasterioxyz-0.0.2/LICENSE
+-rw-r--r--   0        0        0    10095 2024-05-30 15:39:19.266956 rasterioxyz-0.0.2/README.md
+-rw-r--r--   0        0        0      639 2024-05-30 15:39:19.270956 rasterioxyz-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-05-30 15:39:19.270956 rasterioxyz-0.0.2/rasterioxyz/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-30 15:39:19.270956 rasterioxyz-0.0.2/rasterioxyz/_errors.py
+-rw-r--r--   0        0        0     1118 2024-05-30 15:39:19.270956 rasterioxyz-0.0.2/rasterioxyz/_utils.py
+-rw-r--r--   0        0        0    16782 2024-05-30 15:39:19.270956 rasterioxyz-0.0.2/rasterioxyz/tile.py
+-rw-r--r--   0        0        0    10713 1970-01-01 00:00:00.000000 rasterioxyz-0.0.2/PKG-INFO
```

### Comparing `rasterioxyz-0.0.1/LICENSE` & `rasterioxyz-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterioxyz-0.0.1/README.md` & `rasterioxyz-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 ![pypi version](https://img.shields.io/pypi/v/rasterioxyz)
 ![pypi downloads](https://img.shields.io/pypi/dm/rasterioxyz)
 [![publish](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/publish.yaml/badge.svg?branch=main)](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/publish.yaml)
 [![test](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/test.yaml/badge.svg?branch=develop)](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/test.yaml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/8969f1e01f054508bbd7f7d4567e5952)](https://app.codacy.com/gh/duncanmartyn/rasterioxyz/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8969f1e01f054508bbd7f7d4567e5952)](https://app.codacy.com/gh/duncanmartyn/rasterioxyz/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
-![GitHub contributors](https://img.shields.io/github/contributors/duncanmartyn/rasterioxyz)
-![GitHub last commit](https://img.shields.io/github/last-commit/duncanmartyn/rasterioxyz?logo=github)
 
 - [RasterioXYZ](#rasterioxyz)
 - [Introduction](#introduction)
 - [Design](#design)
     - [Memory efficiency](#memory-efficiency)
     - [Flexibility](#flexibility)
 - [Examples](#examples)
   - [Cloud Storage](#cloud-storage)
 - [Benchmarks](#benchmarks)
+  - [Source image (EPSG:32617)](#source-image-epsg32617)
+  - [QGIS-generated tiles](#qgis-generated-tiles)
+  - [RasterioXYZ-generated tiles](#rasterioxyz-generated-tiles)
 - [Roadmap](#roadmap)
     - [High](#high)
     - [Medium](#medium)
     - [Low](#low)
 - [Testing](#testing)
 - [Contributions](#contributions)
 
 # RasterioXYZ
 Package for tiling georeferenced Rasterio DatasetReader objects according to the XYZ tiles standard.
 
 # Introduction
-RasterioXYZ is a lightweight XYZ tile generator depending on the following packages:
-- `rasterio`
-- `numpy`
-
-Written in Python 3.10.11 with Rasterio 1.3.9 and NumPy 1.26.2.
+RasterioXYZ is a lightweight XYZ tile generator written in and depending on the following:
+- `python ^3.10`
+- `rasterio ^1.3.9`
+- `numpy ^1.26.2`
 
 For greater functionality in navigating the tile-tree, see [`Mercantile`](https://github.com/mapbox/mercantile).
 
 # Design
 ### Memory efficiency
 While reprojecting the entire source image at the maximum resolution required, thereof dictated by the maximum zoom level specified, would result in faster tiling, this represents a considerable potential source of memory issues. Such an approach would preclude the tiling of large images, be they large due to spatial resolution, data type, number of bands, and/or area covered. By lazily reading and, if needed, reprojecting windows of the source dataset at a given tile's resolution, memory use is kept low.
 
@@ -45,17 +45,20 @@
 - Tiles need not be generated for all zoom levels in a range
 - Tiles can be saved in PNG or JPEG format, though the XYZ standard dictates the former (as well as lossless and seemingly better colour balancing)
 - Use of any Rasterio recognised resampling technique
 - Creation of standard (256 px) or high (512 px) resolution tiles
 
 # Examples
 ```
+import rasterio
+import rasterioxyz
+
 img = rasterio.open("georeferenced_image.tif")
-tiled = rasterioxyz.Tiles(image=img, zooms=range(10), pixels=256, resampling="bilinear")
-tiles.write("out_directory")
+tiled = rasterioxyz.Tiles(image=img, zooms=range(10), pixels=512, resampling="bilinear")
+tiled.write("out_directory")
 ```
 Several measurements can be taken to improve the speed of tiling:
 - Employ source imagery already projected in EPSG:3857
 - Specify a maximum zoom level at which tile spatial resolution does not greatly exceed that of the source imagery
 - Use the default tile dimensions of 256 pixels
 - Use the default nearest-neighbour resampling
 
@@ -91,31 +94,28 @@
 | QGIS        | 16      | EPSG:3857        | 256                  | 2.06                |
 | QGIS        | 16      | EPSG:3857        | 512                  | 4.96                |
 
 Clearly, QGIS is - at present - many times faster (between 6.6 and 8.7 times). It's likely that some combination of threads, use of lower-level languages, on-the-fly reprojection (in the case of non-3857 images), caching, and pyramids may contribute to QGIS' speed. Potential adoption of threading across bottlenecks (reprojection, writing) is a high priority.
 
 That said, tiles generated by RasterioXYZ appear to exhibit better horizontal accuracy and fewer resampling-derived artefacts than those of QGIS:
 
-![alt text](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport.png "Source image (EPSG:32617)")
-
-Source image (EPSG:32617) without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "Source image, OSM overlay")
-
-![alt text](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport.png "QGIS-tiled zoom level 12")
-
-QGIS-generated tiles without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "QGIS-tiled zoom level 12, OSM overlay")
-
-![alt text](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport.png "RasterioXYZ-tiled zoom level 12")
-
-RasterioXYZ-generated tiles without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "RasterioXYZ-tiled zoom level 12, OSM overlay")
+## Source image (EPSG:32617)
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
+
+## QGIS-generated tiles
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
+
+## RasterioXYZ-generated tiles
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
 
 # Roadmap
 A number of improvements are possible and/or planned. Sorted by priority, these are as follows.
 
 ### High
 - Better handling of non-uint8 datasets with extreme outlying values
   - For example, uint16 Sentinel-2 imagery with extreme outliers in the form of snow or cloud may result in poorly contrasted tiles
@@ -132,26 +132,24 @@
 - Tile data within a user-provided area
 - Enable user selection of raster bands/channels to tile
 - Add command line functionality
 - Enable tiling of sequences of Rasterio datasets
 - Support for colour ramps/tables with singleband images
 
 ### Low
-- A resume/continue mode
+- Resume/continue mode
 - Greater support for different argument values/types (e.g., int/float for resampling)
 - Generate HTML map of tiled data
 
 # Testing
 The test suite for RasterioXYZ uses Rasterio MemoryFile objects containing randomly generated data of specified dtype projected in a specified CRS.
 
 To add additional mock data for testing, do the following in `conftest.py`:
 - Add the target CRS integer to `SUPPORTED_TEST_CRS`
 - Add the target bounding box in said CRS to `TEST_BOUNDS`
 - If desired, change the values for `height`, `width`, and `count` - these are currently hardcoded
 
 Then, in `test_tile.py`:
 - Add the appropriate arguments to the `pytest.mark.parameterize()` decorator for the method to test. For example, after adding EPSG:4269 (NAD83) and a corresponding bounding box, the argument for the `test_data` parameter may appear like so: `{"crs": 4269, "dtype": "uint8"}`
 
-Currently, tests cannot be written to validate the correct tiles (rows and columns) are written by the `write()` method due to said method exhausting the generator of objects containing the requisite information.
-
 # Contributions
 Feel free to raise any issues, especially bugs and feature requests!
```

### Comparing `rasterioxyz-0.0.1/pyproject.toml` & `rasterioxyz-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rasterioxyz"
-version = "0.0.1"
+version = "0.0.2"
 description = "Package for tiling georeferenced rasterio datasets according to the XYZ tiles standard."
 authors = ["Duncan Martyn <duncan.martyn@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `rasterioxyz-0.0.1/rasterioxyz/_utils.py` & `rasterioxyz-0.0.2/rasterioxyz/_utils.py`

 * *Files identical despite different names*

### Comparing `rasterioxyz-0.0.1/rasterioxyz/tile.py` & `rasterioxyz-0.0.2/rasterioxyz/tile.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         "_img_is_3857",
         "_img_properties",
         "_tile_bands",
         "_img_max",
         "_img_min",
         "tiles",
     )
-    _valid_resampling: dict[str, int] = {
+    _valid_resampling = {
         "nearest": 0,
         "bilinear": 1,
         "cubic": 2,
         "cubic_spline": 3,
         "lanczos": 4,
         "average": 5,
         "mode": 6,
@@ -123,15 +123,15 @@
         "min": 9,
         "med": 10,
         "q1": 11,
         "q3": 12,
         "sum": 13,
         "rms": 14,
     }
-    _origin: float = 20037508.342789244
+    _origin = 20037508.342789244
 
     def __init__(
             self,
             image: DatasetReader,
             zooms: Sequence[int] = range(13),
             pixels: int = 256,
             resampling: str = "nearest",
@@ -139,83 +139,81 @@
         if not isinstance(image, DatasetReader):
             raise TypeError(
                 "image must be of type rasterio.DatasetReader, not "
                 f"{type(image).__name__}.",
             )
         if image.crs is None:
             raise errors.CRSError("image must be a georeferenced dataset.")
-        self.img: DatasetReader = image
+        self.img = image
 
         if not isinstance(zooms, Sequence):
             raise TypeError(f"zooms must be a sequence, not {type(zooms).__name__}.")
         if not all(isinstance(zoom, int) for zoom in zooms):
             raise TypeError("all zoom values must be of type int.")
         if not all(zoom <= 25 and zoom >= 0 for zoom in zooms):
             raise ValueError("all zoom values must be between 0 and 25.")
-        self.zooms: Sequence[int] = zooms
+        self.zooms = zooms
 
         if not isinstance(pixels, int):
             raise TypeError(f"pixels must be of type int, not {type(pixels).__name__}.")
         if pixels not in (256, 512):
             raise ValueError(f"pixels must be 256 or 512, not {pixels}.")
-        self.pixels: int = pixels
+        self.pixels = pixels
 
         if not isinstance(resampling, str):
             raise TypeError(
                 f"resampling must be of type str, not {type(resampling).__name__}.",
             )
         if resampling not in self._valid_resampling.keys():
             raise ValueError(
                 f"resampling must be one of {list(self._valid_resampling.keys())}, not "
                 f"{resampling}.",
             )
-        self.resampling: int = self._valid_resampling.get(resampling, 0)
+        self.resampling = self._valid_resampling.get(resampling, 0)
 
-        self._img_is_3857: bool = self.img.crs == 3857
+        self._img_is_3857 = self.img.crs == 3857
         if not self._img_is_3857:
             warnings.warn(
                 f"source CRS is {self.img.crs}. Data will be reprojected to EPSG:3857.",
                 TileWarning,
                 stacklevel=2,
             )
-        self._img_properties: _ImageProperties = self._get_mercator_properties()
+        self._img_properties = self._get_mercator_properties()
 
-        self._tile_bands: int = self.img.count if self.img.count <= 3 else 3
+        self._tile_bands = self.img.count if self.img.count <= 3 else 3
 
-        self._img_dtype: str = self.img.dtypes[0]
+        self._img_dtype = self.img.dtypes[0]
         if self._img_dtype != "uint8":
             warnings.warn(
                 f"source dtype is {self._img_dtype}. Data will be rescaled to uint8.",
                 TileWarning,
                 stacklevel=2,
             )
-            self._img_max: int | float
-            self._img_min: int | float
             self._img_max, self._img_min = self._get_image_statistics()
 
-        self.tiles: Generator[_Tile, None, None] = self._tile()
+        self.tiles = self._tile()
 
     def __repr__(self) -> str:
         """Return a string representation of an instance of Tiles."""
-        resampling_str: str = f"'{list(self._valid_resampling.keys())[self.resampling]}'"
-        message: str = (
+        resampling_str = f"'{list(self._valid_resampling.keys())[self.resampling]}'"
+        message = (
             f"Tiles(image={self.img} zooms={self.zooms} pixels={self.pixels} "
             f"resampling={resampling_str})"
         )
         return message
 
     def __eq__(self, other: Any) -> bool:
         """Test for equality between an instance of Tiles and another object."""
         if not isinstance(other, Tiles):
             return False
 
-        dataset_eq: bool = self.img.profile == other.img.profile
-        zooms_eq: bool = self.zooms == other.zooms
-        pixels_eq: bool = self.pixels == other.pixels
-        resampling_eq: bool = self.resampling == other.resampling
+        dataset_eq = self.img.profile == other.img.profile
+        zooms_eq = self.zooms == other.zooms
+        pixels_eq = self.pixels == other.pixels
+        resampling_eq = self.resampling == other.resampling
 
         if all([dataset_eq, zooms_eq, pixels_eq, resampling_eq]):
             return True
         else:
             return False
 
     def __setattr__(self, name: str, value: Any) -> None:
@@ -230,35 +228,31 @@
         source rasterio dataset, returning an _ImageProperties object thereof.
 
         Returns
         -------
         properties : _ImageProperties
             _ImageProperties object corresponding to the source rasterio dataset.
         """
-        properties: _ImageProperties
         if self._img_is_3857:
             properties = _ImageProperties(
                 self.img.transform,
                 _Bounds(*self.img.bounds),
             )
         else:
-            transform: Affine
-            width: int
-            height: int
             transform, width, height = warp.calculate_default_transform(
                 self.img.crs,
                 3857,
                 self.img.width,
                 self.img.height,
                 *self.img.bounds,
             )
-            minx: float = transform[2]
-            maxx: float = minx + transform[0] * width
-            maxy: float = transform[5]
-            miny: float = maxy + transform[4] * height
+            minx = transform[2]
+            maxx = minx + transform[0] * width
+            maxy = transform[5]
+            miny = maxy + transform[4] * height
             properties = _ImageProperties(
                 transform,
                 _Bounds(minx, miny, maxx, maxy),
             )
         return properties
 
     def _get_image_statistics(self) -> tuple[int | float, int | float]:
@@ -269,34 +263,34 @@
         Returns
         -------
         img_max : int | float
             Maximum value across all bands of the source dataset.
         img_min : int | float
             Minimum value across all bands of the source dataset.
         """
-        band_statistics: list[Any] = [
+        band_statistics = [
             self.img.statistics(band) for band in range(1, self._tile_bands + 1)
         ]
-        img_max: int | float = max([stats.max for stats in band_statistics])
-        img_min: int | float = min([stats.min for stats in band_statistics])
+        img_max = max([stats.max for stats in band_statistics])
+        img_min = min([stats.min for stats in band_statistics])
         return img_max, img_min
 
     def _tile(self) -> Generator[_Tile, None, None]:
         """
         Generate _Tile objects for the instance's rasterio dataset and zooms.
 
         Yields
         ------
         tile : _Tile
             _Tile object corresponding to a single XYZ tile.
         """
         for zoom in self.zooms:
-            zoom_properties: _Zoom = self._build_zoom(zoom)
+            zoom_properties = self._build_zoom(zoom)
             for col, row in zoom_properties.tile_indices:
-                tile: _Tile = self._build_tile(zoom, col, row, zoom_properties.tile_dims)
+                tile = self._build_tile(zoom, col, row, zoom_properties.tile_dims)
 
                 yield tile
 
     def _build_zoom(self, zoom: int) -> _Zoom:
         """
         Generate a _Zoom object corresponding to a single XYZ zoom level.
 
@@ -306,44 +300,38 @@
             Zoom level for which to generate a _Zoom object.
 
         Returns
         -------
         tile : _Tile
             _Zoom object corresponding to a single XYZ zoom level.
         """
-        zoom_ntiles: int = 4 ** zoom
-        zoom_dims: float = zoom_ntiles ** .5
-        tile_dims: float = (self._origin * 2) / zoom_dims
-        tile_res: float = tile_dims / self.pixels
+        zoom_ntiles = 4 ** zoom
+        zoom_dims = zoom_ntiles ** .5
+        tile_dims = (self._origin * 2) / zoom_dims
+        tile_res = tile_dims / self.pixels
         if tile_res < self._img_properties.transform[0]:
             warnings.warn(
                 f"tile resolution is higher than source at zoom level {zoom}. "
                 "Consider reducing maximum zoom level for better performance.",
                 TileWarning,
                 stacklevel=3,
             )
-
-        start_col: int = int(
-            (self._origin - abs(self._img_properties.bounds.minx)) // tile_dims,
-        )
-        end_col: int = int(
-            (self._origin - abs(self._img_properties.bounds.maxx)) // tile_dims,
-        )
-        start_row: int = int(
-            (self._origin - abs(self._img_properties.bounds.maxy)) // tile_dims,
+        start_col = int((self._img_properties.bounds.minx - -self._origin) // tile_dims)
+        end_col = int((self._img_properties.bounds.maxx - -self._origin) // tile_dims)
+        start_row = int(
+            abs(self._img_properties.bounds.maxy - self._origin) // tile_dims,
         )
-        end_row: int = int(
-            (self._origin - abs(self._img_properties.bounds.miny)) // tile_dims,
+        end_row = int(
+            abs(self._img_properties.bounds.miny - self._origin) // tile_dims,
         )
-        tile_indices: product = product(
+        tile_indices = product(
             range(start_col, end_col + 1),
             range(start_row, end_row + 1),
         )
-
-        zoom_properties: _Zoom = _Zoom(zoom, tile_dims, tile_indices)
+        zoom_properties = _Zoom(zoom, tile_dims, tile_indices)
         return zoom_properties
 
     def _build_tile(self, zoom: int, col: int, row: int, dims: int | float) -> _Tile:
         """
         Generate a _Tile object corresponding to a single XYZ tile.
 
         Parameters
@@ -358,37 +346,33 @@
             Tile to generate's height/width in metres.
 
         Returns
         -------
         tile : _Tile
             _Tile object corresponding to a single XYZ tile.
         """
-        minx: float = self._origin * -1 + col * dims
-        maxx: float = minx + dims
-        maxy: float = self._origin - row * dims
-        miny: float = maxy - dims
-        bounds: _Bounds = _Bounds(minx, miny, maxx, maxy)
-        trans: Affine = transform.from_bounds(*bounds, self.pixels, self.pixels)
-        window: windows.Window = windows.from_bounds(
-            *bounds,
-            self._img_properties.transform,
-        )
-        tile_data: ndarray
+        minx = self._origin * -1 + col * dims
+        maxx = minx + dims
+        maxy = self._origin - row * dims
+        miny = maxy - dims
+        bounds = _Bounds(minx, miny, maxx, maxy)
+        affine = transform.from_bounds(*bounds, self.pixels, self.pixels)
+        window = windows.from_bounds(*bounds, self._img_properties.transform)
         if self._img_is_3857:
             tile_data = self._read_tile_data(window)
         else:
-            tile_data = self._reproject_tile_data(window, trans)
+            tile_data = self._reproject_tile_data(window, affine)
         if tile_data.dtype != uint8:
             tile_data = self._array_to_uint8(tile_data)
-        tile: _Tile = _Tile(
+        tile = _Tile(
             zoom=zoom,
             column=col,
             row=row,
             bounds=bounds,
-            transform=trans,
+            transform=affine,
             window=window,
             data=tile_data,
         )
         return tile
 
     def _reproject_tile_data(
             self,
@@ -404,15 +388,15 @@
             Tile object for which data will be read.
 
         Returns
         -------
         tile_array : numpy.ndarray
             Data within the tile's window.
         """
-        tile_array: ndarray = warp.reproject(
+        tile_array = warp.reproject(
             source=Band(
                 self.img,
                 range(1, self._tile_bands + 1),
                 dtype=self._img_dtype,
                 shape=(tile_window.height, tile_window.width),
             ),
             destination=zeros(
@@ -439,22 +423,22 @@
             Tile object for which data will be read.
 
         Returns
         -------
         tile_array : numpy.ndarray
             Data within the tile's window.
         """
-        tile_array: ndarray = self.img.read(
+        tile_array = self.img.read(
             out_shape=(self._tile_bands, self.pixels, self.pixels),
             window=tile_window,
             masked=True,
             boundless=True,
             resampling=self.resampling,
         )
-        tile_alpha: ndarray = where(
+        tile_alpha = where(
             tile_array[0].mask, 0, 255
         ).reshape((1, self.pixels, self.pixels)).astype(self._img_dtype)
         tile_array = append(tile_array, tile_alpha, axis=0)
         return tile_array
 
     def _array_to_uint8(self, tile_array: ndarray) -> ndarray:
         """
@@ -467,15 +451,14 @@
             Array to rescale and cast to uint8.
 
         Returns
         -------
         rescaled_array : numpy.ndarray
             Rescaled uint8 array.
         """
-        # rescale all bands but alpha
         tile_array[:-1] = (
             (tile_array[:-1] - self._img_min) / (self._img_max - self._img_min)
         ) * (255 - 0) + 0
         tile_array = tile_array.astype(uint8)
         return tile_array
 
     def write(self, directory: str | Path, driver: str = "PNG") -> None:
@@ -493,22 +476,22 @@
         warnings.filterwarnings("ignore", category=errors.NotGeoreferencedWarning)
 
         if not isinstance(driver, (str, Path)):
             raise TypeError(f"driver must be str or Path, not {type(driver)}.")
         if driver.upper() not in ["PNG", "JPEG"]:
             raise ValueError(f"driver must be PNG or JPEG, not {driver}.")
 
-        out_dir: Path = Path(directory) if not isinstance(directory, Path) else directory
+        out_dir = Path(directory) if not isinstance(directory, Path) else directory
         if not out_dir.exists() or not out_dir.is_dir():
             raise FileNotFoundError(f"directory does not exist: {directory}")
 
         for tile in self.tiles:
-            img_dir: Path = out_dir.joinpath(str(tile.zoom), str(tile.column))
+            img_dir = out_dir.joinpath(str(tile.zoom), str(tile.column))
             img_dir.mkdir(parents=True, exist_ok=True)
-            img_path: Path = img_dir.joinpath(f"{tile.row}.{driver}")
+            img_path = img_dir.joinpath(f"{tile.row}.{driver}")
 
             # if alpha indicates total transparency, skip write
             if tile.data[-1].mean() == 0:
                 continue
 
             with ropen(
                 img_path,
```

### Comparing `rasterioxyz-0.0.1/PKG-INFO` & `rasterioxyz-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterioxyz
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for tiling georeferenced rasterio datasets according to the XYZ tiles standard.
 License: MIT
 Author: Duncan Martyn
 Author-email: duncan.martyn@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,41 +18,41 @@
 ![pypi version](https://img.shields.io/pypi/v/rasterioxyz)
 ![pypi downloads](https://img.shields.io/pypi/dm/rasterioxyz)
 [![publish](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/publish.yaml/badge.svg?branch=main)](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/publish.yaml)
 [![test](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/test.yaml/badge.svg?branch=develop)](https://github.com/duncanmartyn/rasterioxyz/actions/workflows/test.yaml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/8969f1e01f054508bbd7f7d4567e5952)](https://app.codacy.com/gh/duncanmartyn/rasterioxyz/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/8969f1e01f054508bbd7f7d4567e5952)](https://app.codacy.com/gh/duncanmartyn/rasterioxyz/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
-![GitHub contributors](https://img.shields.io/github/contributors/duncanmartyn/rasterioxyz)
-![GitHub last commit](https://img.shields.io/github/last-commit/duncanmartyn/rasterioxyz?logo=github)
 
 - [RasterioXYZ](#rasterioxyz)
 - [Introduction](#introduction)
 - [Design](#design)
     - [Memory efficiency](#memory-efficiency)
     - [Flexibility](#flexibility)
 - [Examples](#examples)
   - [Cloud Storage](#cloud-storage)
 - [Benchmarks](#benchmarks)
+  - [Source image (EPSG:32617)](#source-image-epsg32617)
+  - [QGIS-generated tiles](#qgis-generated-tiles)
+  - [RasterioXYZ-generated tiles](#rasterioxyz-generated-tiles)
 - [Roadmap](#roadmap)
     - [High](#high)
     - [Medium](#medium)
     - [Low](#low)
 - [Testing](#testing)
 - [Contributions](#contributions)
 
 # RasterioXYZ
 Package for tiling georeferenced Rasterio DatasetReader objects according to the XYZ tiles standard.
 
 # Introduction
-RasterioXYZ is a lightweight XYZ tile generator depending on the following packages:
-- `rasterio`
-- `numpy`
-
-Written in Python 3.10.11 with Rasterio 1.3.9 and NumPy 1.26.2.
+RasterioXYZ is a lightweight XYZ tile generator written in and depending on the following:
+- `python ^3.10`
+- `rasterio ^1.3.9`
+- `numpy ^1.26.2`
 
 For greater functionality in navigating the tile-tree, see [`Mercantile`](https://github.com/mapbox/mercantile).
 
 # Design
 ### Memory efficiency
 While reprojecting the entire source image at the maximum resolution required, thereof dictated by the maximum zoom level specified, would result in faster tiling, this represents a considerable potential source of memory issues. Such an approach would preclude the tiling of large images, be they large due to spatial resolution, data type, number of bands, and/or area covered. By lazily reading and, if needed, reprojecting windows of the source dataset at a given tile's resolution, memory use is kept low.
 
@@ -62,17 +62,20 @@
 - Tiles need not be generated for all zoom levels in a range
 - Tiles can be saved in PNG or JPEG format, though the XYZ standard dictates the former (as well as lossless and seemingly better colour balancing)
 - Use of any Rasterio recognised resampling technique
 - Creation of standard (256 px) or high (512 px) resolution tiles
 
 # Examples
 ```
+import rasterio
+import rasterioxyz
+
 img = rasterio.open("georeferenced_image.tif")
-tiled = rasterioxyz.Tiles(image=img, zooms=range(10), pixels=256, resampling="bilinear")
-tiles.write("out_directory")
+tiled = rasterioxyz.Tiles(image=img, zooms=range(10), pixels=512, resampling="bilinear")
+tiled.write("out_directory")
 ```
 Several measurements can be taken to improve the speed of tiling:
 - Employ source imagery already projected in EPSG:3857
 - Specify a maximum zoom level at which tile spatial resolution does not greatly exceed that of the source imagery
 - Use the default tile dimensions of 256 pixels
 - Use the default nearest-neighbour resampling
 
@@ -108,31 +111,28 @@
 | QGIS        | 16      | EPSG:3857        | 256                  | 2.06                |
 | QGIS        | 16      | EPSG:3857        | 512                  | 4.96                |
 
 Clearly, QGIS is - at present - many times faster (between 6.6 and 8.7 times). It's likely that some combination of threads, use of lower-level languages, on-the-fly reprojection (in the case of non-3857 images), caching, and pyramids may contribute to QGIS' speed. Potential adoption of threading across bottlenecks (reprojection, writing) is a high priority.
 
 That said, tiles generated by RasterioXYZ appear to exhibit better horizontal accuracy and fewer resampling-derived artefacts than those of QGIS:
 
-![alt text](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport.png "Source image (EPSG:32617)")
-
-Source image (EPSG:32617) without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "Source image, OSM overlay")
-
-![alt text](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport.png "QGIS-tiled zoom level 12")
-
-QGIS-generated tiles without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "QGIS-tiled zoom level 12, OSM overlay")
-
-![alt text](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport.png "RasterioXYZ-tiled zoom level 12")
-
-RasterioXYZ-generated tiles without (T) and with (B) OSM overlay.
-
-![alt text](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport_OSM_overlay.png "RasterioXYZ-tiled zoom level 12, OSM overlay")
+## Source image (EPSG:32617)
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/Sentinel2_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
+
+## QGIS-generated tiles
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/QGIS_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
+
+## RasterioXYZ-generated tiles
+| Without OSM | With OSM |
+| :-: | :-: |
+| ![](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport.png) | ![](doc/gallery/RasterioXYZ_T17RLK_Venice_Municipal_Airport_OSM_overlay.png) |
 
 # Roadmap
 A number of improvements are possible and/or planned. Sorted by priority, these are as follows.
 
 ### High
 - Better handling of non-uint8 datasets with extreme outlying values
   - For example, uint16 Sentinel-2 imagery with extreme outliers in the form of snow or cloud may result in poorly contrasted tiles
@@ -149,27 +149,25 @@
 - Tile data within a user-provided area
 - Enable user selection of raster bands/channels to tile
 - Add command line functionality
 - Enable tiling of sequences of Rasterio datasets
 - Support for colour ramps/tables with singleband images
 
 ### Low
-- A resume/continue mode
+- Resume/continue mode
 - Greater support for different argument values/types (e.g., int/float for resampling)
 - Generate HTML map of tiled data
 
 # Testing
 The test suite for RasterioXYZ uses Rasterio MemoryFile objects containing randomly generated data of specified dtype projected in a specified CRS.
 
 To add additional mock data for testing, do the following in `conftest.py`:
 - Add the target CRS integer to `SUPPORTED_TEST_CRS`
 - Add the target bounding box in said CRS to `TEST_BOUNDS`
 - If desired, change the values for `height`, `width`, and `count` - these are currently hardcoded
 
 Then, in `test_tile.py`:
 - Add the appropriate arguments to the `pytest.mark.parameterize()` decorator for the method to test. For example, after adding EPSG:4269 (NAD83) and a corresponding bounding box, the argument for the `test_data` parameter may appear like so: `{"crs": 4269, "dtype": "uint8"}`
 
-Currently, tests cannot be written to validate the correct tiles (rows and columns) are written by the `write()` method due to said method exhausting the generator of objects containing the requisite information.
-
 # Contributions
 Feel free to raise any issues, especially bugs and feature requests!
```

