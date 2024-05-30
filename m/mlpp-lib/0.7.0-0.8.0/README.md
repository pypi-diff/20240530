# Comparing `tmp/mlpp_lib-0.7.0.tar.gz` & `tmp/mlpp_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpp_lib-0.7.0.tar", max compression
+gzip compressed data, was "mlpp_lib-0.8.0.tar", max compression
```

## Comparing `mlpp_lib-0.7.0.tar` & `mlpp_lib-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1518 2024-03-21 15:39:15.741873 mlpp_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0     7155 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/README.md
--rw-r--r--   0        0        0       22 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/__init__.py
--rw-r--r--   0        0        0     1624 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/callbacks.py
--rw-r--r--   0        0        0    25322 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/datasets.py
--rw-r--r--   0        0        0      444 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/decorators.py
--rw-r--r--   0        0        0     5747 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/ensemble.py
--rw-r--r--   0        0        0    21716 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/losses.py
--rw-r--r--   0        0        0     1179 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/metrics.py
--rw-r--r--   0        0        0    22103 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/model_selection.py
--rw-r--r--   0        0        0    16989 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/models.py
--rw-r--r--   0        0        0     2048 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/physical_layers.py
--rw-r--r--   0        0        0    29932 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/probabilistic_layers.py
--rw-r--r--   0        0        0     3957 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/standardizers.py
--rw-r--r--   0        0        0     4309 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/train.py
--rw-r--r--   0        0        0     7086 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/mlpp_lib/utils.py
--rw-r--r--   0        0        0      988 2024-03-21 15:39:15.745873 mlpp_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 mlpp_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-05-30 08:40:51.226262 mlpp_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7155 2024-05-30 08:40:51.226262 mlpp_lib-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-30 08:40:51.226262 mlpp_lib-0.8.0/mlpp_lib/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-30 08:40:51.226262 mlpp_lib-0.8.0/mlpp_lib/callbacks.py
+-rw-r--r--   0        0        0    25107 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/datasets.py
+-rw-r--r--   0        0        0      444 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/decorators.py
+-rw-r--r--   0        0        0     5747 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/ensemble.py
+-rw-r--r--   0        0        0    21716 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/losses.py
+-rw-r--r--   0        0        0     1179 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/metrics.py
+-rw-r--r--   0        0        0    22930 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/model_selection.py
+-rw-r--r--   0        0        0    16989 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/models.py
+-rw-r--r--   0        0        0     2048 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/physical_layers.py
+-rw-r--r--   0        0        0    29932 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/probabilistic_layers.py
+-rw-r--r--   0        0        0     3957 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/standardizers.py
+-rw-r--r--   0        0        0     4309 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/train.py
+-rw-r--r--   0        0        0     7086 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/mlpp_lib/utils.py
+-rw-r--r--   0        0        0      988 2024-05-30 08:40:51.230262 mlpp_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 mlpp_lib-0.8.0/PKG-INFO
```

### Comparing `mlpp_lib-0.7.0/LICENSE` & `mlpp_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/README.md` & `mlpp_lib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/callbacks.py` & `mlpp_lib-0.8.0/mlpp_lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/datasets.py` & `mlpp_lib-0.8.0/mlpp_lib/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,17 @@
             If "test", only testing data is processed.
             If None, all data is processed.
         """
         LOGGER.info(f"Beginning datamodule setup for stage='{stage}'")
         maybe_load = self._check_args()
         if maybe_load:
             self.load_raw()
-        self.select_splits(stage=stage)
         if self.filter is not None:
-            self.apply_filter(stage=stage)
+            self.apply_filter()
+        self.select_splits(stage=stage)
         self.standardize(stage=stage)
         self.as_datasets(stage=stage)
 
     def load_raw(self):
         LOGGER.info(f"Loading data from: {self.data_dir}")
 
         self.x = (
@@ -145,21 +145,17 @@
                 *args, partition="val", thinning=self.thinning
             )
         if stage == "test" or stage is None:
             self.test = self.splitter.get_partition(
                 *args, partition="test", thinning=self.thinning
             )
 
-    def apply_filter(self, stage=None):
+    def apply_filter(self):
         LOGGER.info("Applying filter to features and targets.")
-        if stage == "fit" or stage is None:
-            self.train = self.filter.apply(*self.train)
-            self.val = self.filter.apply(*self.val)
-        if stage == "test" or stage is None:
-            self.test = self.filter.apply(*self.test)
+        self.x, self.y = self.filter.apply(self.x, self.y)
 
     def standardize(self, stage=None):
         LOGGER.info("Standardizing data.")
         if self.standardizer is None:
             if stage == "test":
                 raise ValueError("Must provide standardizer for `test` stage.")
```

### Comparing `mlpp_lib-0.7.0/mlpp_lib/ensemble.py` & `mlpp_lib-0.8.0/mlpp_lib/ensemble.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/losses.py` & `mlpp_lib-0.8.0/mlpp_lib/losses.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/metrics.py` & `mlpp_lib-0.8.0/mlpp_lib/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/model_selection.py` & `mlpp_lib-0.8.0/mlpp_lib/model_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,36 @@
             )
         self.partition_names = list(time_split.keys())
         self._check_time(time_split, time_split_method)
         self._check_station(station_split, station_split_method)
         self.seed = seed
         self.time_dim_name = time_dim_name
 
+    def fit(self, *args: xr.Dataset) -> Self:
+        """Compute splits based on the input datasets.
+
+        Parameters
+        ----------
+        *args: `xr.Dataset`
+            The datasets defining the time and station indices.
+
+        Returns
+        -------
+        self: `DataSplitter`
+            The fitted DataSplitter instance.
+        """
+
+        self.time_index = args[0][self.time_dim_name].values.copy()
+        self.station_index = args[0].station.values.copy()
+
+        self._time_partitioning()
+        self._station_partitioning()
+
+        return self
+
     def get_partition(
         self, *args: xr.Dataset, partition=None, thinning: Optional[Mapping] = None
     ) -> tuple[xr.Dataset, ...]:
         """
         Select and return a partition based on the current values in
         the `partitions` attribute.
 
@@ -137,19 +159,16 @@
         partition: tuple of `xr.Dataset`
             Subsets of the input datasets.
         """
 
         if partition is None:
             raise ValueError("Keyword argument `partition` must be provided.")
 
-        self.time_index = args[0][self.time_dim_name].values.copy()
-        self.station_index = args[0].station.values.copy()
-
-        self._time_partitioning()
-        self._station_partitioning()
+        if not hasattr(self, "time_index") or not hasattr(self, "station_index"):
+            self = self.fit(*args)
 
         # avoid out-of-order indexing (leads to bad performance with xarray/dask)
         station_idx = self.partitions[partition]["station"]
         idx_loc = [pd.Index(self.station_index).get_loc(label) for label in station_idx]
         self.partitions[partition]["station"] = list(
             np.array(station_idx)[np.argsort(idx_loc)]
         )
@@ -190,15 +209,18 @@
                 res = self._time_partition_method(_time_split)
                 self._time_indexers.update(res)
 
         # assign indexers
         for partition in self.partition_names:
             idx = self._time_indexers[partition]
             idx = pd.to_datetime(idx)  # always convert to pandas datetime indices
-            idx = slice(*idx) if len(idx) == 2 else idx
+            if len(idx) == 2:
+                # convert slice to list of labels
+                time_index = pd.to_datetime(self.time_index)
+                idx = time_index[time_index.slice_indexer(start=idx[0], end=idx[1])]
             indexer = {self.time_dim_name: idx}
             if not hasattr(self, "partitions"):
                 self.partitions = {p: {} for p in self.partition_names}
             self.partitions[partition].update(indexer)
 
     def _time_partition_method(self, fractions: Mapping[str, float]):
         if self.time_split_method == "sequential":
@@ -285,27 +307,29 @@
         splitter = cls(time_split, station_split)
         splitter._time_defined = True
         splitter._station_defined = True
         splitter._time_partitioning()
         splitter._station_partitioning()
         return splitter
 
-    def to_dict(self):
+    def to_dict(self, sort_values=False):
         if not hasattr(self, "time_index") or not hasattr(self, "station_index"):
-            raise ValueError("DataSplitter wasn't applied on data yet")
+            raise ValueError("DataSplitter wasn't applied on any data yet, run `fit` first.")
         if not hasattr(self, "partitions"):
             self._time_partitioning()
             self._station_partitioning()
         partitions = deepcopy(self.partitions)
         for split_key, split_dict in partitions.items():
             for dim, value in split_dict.items():
                 if isinstance(value, slice):
                     partitions[split_key][dim] = [str(value.start), str(value.stop)]
                 elif hasattr(value, "tolist"):
                     partitions[split_key][dim] = value.astype(str).tolist()
+                    if sort_values:
+                        partitions[split_key][dim] = sorted(partitions[split_key][dim])
         return partitions
 
     @classmethod
     def from_json(cls, in_fn: str) -> Self:
         with open(in_fn, "r") as f:
             in_dict = json.load(f)
         return cls.from_dict(in_dict)
```

### Comparing `mlpp_lib-0.7.0/mlpp_lib/models.py` & `mlpp_lib-0.8.0/mlpp_lib/models.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/physical_layers.py` & `mlpp_lib-0.8.0/mlpp_lib/physical_layers.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/probabilistic_layers.py` & `mlpp_lib-0.8.0/mlpp_lib/probabilistic_layers.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/standardizers.py` & `mlpp_lib-0.8.0/mlpp_lib/standardizers.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/train.py` & `mlpp_lib-0.8.0/mlpp_lib/train.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/mlpp_lib/utils.py` & `mlpp_lib-0.8.0/mlpp_lib/utils.py`

 * *Files identical despite different names*

### Comparing `mlpp_lib-0.7.0/pyproject.toml` & `mlpp_lib-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpp-lib"
-version = "0.7.0"
+version = "0.8.0"
 description = "Collection of methods for ML-based postprocessing of weather forecasts."
 authors = ["Daniele Nerini <daniele.nerini@meteoswiss.ch>"]
 include = ["LICENSE", "README.md"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
 numpy = "^1.22.1"
```

### Comparing `mlpp_lib-0.7.0/PKG-INFO` & `mlpp_lib-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpp-lib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Collection of methods for ML-based postprocessing of weather forecasts.
 Author: Daniele Nerini
 Author-email: daniele.nerini@meteoswiss.ch
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

