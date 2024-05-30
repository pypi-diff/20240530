# Comparing `tmp/dongraphio-0.3.8.tar.gz` & `tmp/dongraphio-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.8.tar", max compression
+gzip compressed data, was "dongraphio-0.3.9.tar", max compression
```

## Comparing `dongraphio-0.3.8.tar` & `dongraphio-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1498 2024-05-23 10:26:37.987404 dongraphio-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0     1424 2024-05-23 11:11:22.740104 dongraphio-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1461 2024-05-23 10:26:37.982852 dongraphio-0.3.8/README.md
--rw-r--r--   0        0        0      211 2024-05-23 11:09:43.856243 dongraphio-0.3.8/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14870 2024-05-23 10:26:37.735216 dongraphio-0.3.8/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     5446 2024-05-23 11:09:43.856243 dongraphio-0.3.8/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2750 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     5626 2024-05-23 10:26:37.735216 dongraphio-0.3.8/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/enums.py
--rw-r--r--   0        0        0      466 2024-05-23 10:26:37.703963 dongraphio-0.3.8/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19279 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2606 2024-05-23 10:26:37.719589 dongraphio-0.3.8/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-05-23 10:26:37.703963 dongraphio-0.3.8/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1738 2024-05-23 10:26:37.703963 dongraphio-0.3.8/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 dongraphio-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-30 14:21:03.634967 dongraphio-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     1424 2024-05-30 14:21:03.640969 dongraphio-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1461 2024-05-30 14:21:03.631966 dongraphio-0.3.9/README.md
+-rw-r--r--   0        0        0      211 2024-05-30 14:21:03.419785 dongraphio-0.3.9/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-30 14:21:03.423786 dongraphio-0.3.9/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14870 2024-05-30 14:21:03.428788 dongraphio-0.3.9/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5715 2024-05-30 14:21:03.430789 dongraphio-0.3.9/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2750 2024-05-30 14:21:03.425787 dongraphio-0.3.9/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     5626 2024-05-30 14:21:03.432788 dongraphio-0.3.9/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-05-30 14:21:03.418786 dongraphio-0.3.9/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      466 2024-05-30 14:21:03.406782 dongraphio-0.3.9/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-30 14:21:03.416785 dongraphio-0.3.9/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19279 2024-05-30 14:21:03.412785 dongraphio-0.3.9/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2606 2024-05-30 14:21:03.414784 dongraphio-0.3.9/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-05-30 14:21:03.407782 dongraphio-0.3.9/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1738 2024-05-30 14:21:03.409784 dongraphio-0.3.9/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 dongraphio-0.3.9/PKG-INFO
```

### Comparing `dongraphio-0.3.8/LICENSE.txt` & `dongraphio-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/pyproject.toml` & `dongraphio-0.3.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dongraphio"
-version = "0.3.8"
+version = "0.3.9"
 license = "BSD-3-Clause"
 description = "Small utility library containing graph algorighms used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "dongraphio", from = "src" }]
```

### Comparing `dongraphio-0.3.8/README.md` & `dongraphio-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.9/src/dongraphio/base_models/grapher_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.9/src/dongraphio/base_models/isochrones_logic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Literal, Optional, Tuple
 
 import geopandas as gpd
-import networkit as nk
 import networkx as nx
 import pandas as pd
 from loguru import logger
 from pydantic import BaseModel, InstanceOf, field_validator
 from shapely import Point, from_wkt
 from shapely.ops import unary_union
 from tqdm.auto import tqdm
 
 from ..enums import GraphType
-from ..utils import convert_multidigraph_to_digraph, get_nx2nk_idmap, matrix_utils, nx_to_gdf
+from ..utils import convert_multidigraph_to_digraph, matrix_utils, nx_to_gdf
+from ..utils.matrix_utils import get_dist_matrix
 
 tqdm.pandas()
 
 
 class BuildsAvailabilitier(BaseModel):
     graph_type: list[GraphType]
     city_crs: int
@@ -47,74 +47,84 @@
 
         if mobility_graph.is_multigraph() & mobility_graph.is_directed():
             mobility_graph = convert_multidigraph_to_digraph(mobility_graph, self.weight_type)
         mobility_graph.graph["crs"] = self.city_crs
         graph_gdf = nx_to_gdf(nx.MultiDiGraph(mobility_graph), nodes=True)
 
         from_sources = graph_gdf["geometry"].sindex.nearest(self.points, return_distance=True, return_all=False)
+        dist_nearest = pd.DataFrame(data=from_sources[1], index=from_sources[0][1], columns=["dist"])
+        walk_speed = 4 * 1000 / 60
+        dist_nearest = dist_nearest / walk_speed if self.weight_type == "time_min" else dist_nearest
+
+        if (dist_nearest > self.weight_value).all().all():
+            raise RuntimeError(
+                "The point(s) lie further from the graph than weight_value, it's impossible to "
+                "construct isochrones. Check the coordinates of the point(s)/their projection"
+            )
+
         source_index = from_sources[0][1]
         distances = pd.DataFrame(float(0), index=source_index, columns=list(mobility_graph.nodes()))
 
         logger.debug("Calculating distances from the specified point...")
 
-        mapping = get_nx2nk_idmap(mobility_graph)
-        nk_graph = nk.nxadapter.nx2nk(mobility_graph, self.weight_type)
-        spsp = nk.distance.SPSP(G=nk_graph, sources=distances.index.values).run()
-        for index, _ in distances.iterrows():
-            for column in distances.columns:
-                distances.loc[index, column] = spsp.getDistance(mapping.get(index), mapping.get(column))
-        del spsp
+        distances = get_dist_matrix(
+            mobility_graph, source_index, distances.columns.values, path_matrix=False, weight=self.weight_type
+        )
 
-        dist_nearest = pd.DataFrame(data=from_sources[1], index=from_sources[0][1], columns=["dist"])
-        walk_speed = 4 * 1000 / 60
-        dist_nearest = dist_nearest / walk_speed if self.weight_type == "time_min" else dist_nearest
         distances = distances.add(dist_nearest.dist, axis=0).transpose()
 
         distances = distances[distances[source_index] <= self.weight_value]
+        distances.dropna(how="all", inplace=True)
+
         results = []
         point_num = 0
         logger.debug("Building isochrones geometry...")
         for column_name in distances.columns:
             geometry = []
             for ind in distances.index:
                 value = distances.loc[ind, column_name]
                 if not pd.isna(value):
                     geometry.append(
                         graph_gdf.loc[ind].geometry.buffer(round(self.weight_value - value, 2) * walk_speed * 0.8)
                         if self.weight_type == "time_min"
                         else graph_gdf.loc[ind].geometry.buffer(round(self.weight_value - value, 2) * 0.8)
                     )
             geometry = unary_union(geometry)
-            results.append({"geometry": geometry, "point": str(self.points.iloc[point_num])})
+            results.append({"geometry": geometry, "point": str(self.points.iloc[point_num]), "point_number": point_num})
             point_num += 1
 
         isochrones = gpd.GeoDataFrame(data=results, geometry="geometry", crs=self.city_crs)
         isochrones["travel_type"] = str([d.russian_name for d in self.graph_type])
         isochrones["weight_type"] = self.weight_type
         isochrones["weight_value"] = self.weight_value
 
         stops, routes = (None, None)
         if GraphType.PUBLIC_TRANSPORT in self.graph_type and self.weight_type == "time_min":
             if not (graph_gdf[graph_gdf["stop"] == "True"]).empty:
-                stops, routes = self._get_routes(graph_gdf, distances.index.values, mobility_graph)
+                stops, routes = self._get_routes(graph_gdf, distances, mobility_graph)
             else:
                 logger.info("No public transport node in graph")
         return isochrones, routes, stops
 
-    def _get_routes(self, graph_gdf, selected_nodes, mobility_graph):
-        stops = graph_gdf[graph_gdf["stop"] == "True"]
+    def _get_routes(self, graph_gdf, distances, mobility_graph):
+        selected_nodes = distances.index.values
+        stops = graph_gdf.loc[selected_nodes]
+        stops = stops[stops["stop"] == "True"]
+
         stop_types = (
             stops["desc"]
             .astype(object)
             .apply(lambda x: pd.Series({t: True for t in x.split(", ")}))
             .astype(bool)
             .fillna(False)
             .infer_objects(copy=False)
         )
         stops = stops.join(stop_types)
         selected_nodes = [node for node in selected_nodes if node in stops.index]
         subgraph = mobility_graph.subgraph(selected_nodes)
         routes = pd.DataFrame.from_records([e[-1] for e in subgraph.edges(data=True)])
-        routes["geometry"] = routes["geometry"].apply(from_wkt)
+        if routes.empty:
+            return None, None
+        routes["geometry"] = routes["geometry"].apply(lambda x: from_wkt(str(x)))
         routes_result = gpd.GeoDataFrame(data=routes, geometry="geometry", crs=graph_gdf.crs)
         stops_result = gpd.GeoDataFrame(data=stops.loc[selected_nodes], geometry="geometry", crs=graph_gdf.crs)
         return stops_result, routes_result
```

### Comparing `dongraphio-0.3.8/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.9/src/dongraphio/base_models/matrix_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/dongraphio.py` & `dongraphio-0.3.9/src/dongraphio/dongraphio.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/enums.py` & `dongraphio-0.3.9/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.9/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.9/src/dongraphio/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.9/src/dongraphio/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.9/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.9/src/dongraphio/utils/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.8/PKG-INFO` & `dongraphio-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.8
+Version: 0.3.9
 Summary: Small utility library containing graph algorighms used in other projects
 License: BSD-3-Clause
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

