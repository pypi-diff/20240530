# Comparing `tmp/pycitysim-1.15.0.tar.gz` & `tmp/pycitysim-1.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycitysim-1.15.0.tar", last modified: Mon May 27 16:35:26 2024, max compression
+gzip compressed data, was "pycitysim-1.15.1.tar", last modified: Thu May 30 06:14:19 2024, max compression
```

## Comparing `pycitysim-1.15.0.tar` & `pycitysim-1.15.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.540776 pycitysim-1.15.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 16:35:21.000000 pycitysim-1.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-27 16:35:26.540776 pycitysim-1.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-27 16:35:21.000000 pycitysim-1.15.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.532776 pycitysim-1.15.0/pycitysim/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/apphub/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/apphub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/apphub/apphub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/map/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37630 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/map/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/routing/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/sateimg/
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sateimg/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sateimg/sateimg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sidecar/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/aoi_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/clock_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/economy_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/lane_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/light_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/person_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/road_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/sim/social_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.536776 pycitysim-1.15.0/pycitysim/streetview/
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/streetview/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/streetview/equirectangular.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/streetview/google.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.540776 pycitysim-1.15.0/pycitysim/urbankg/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/urbankg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/urbankg/kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.540776 pycitysim-1.15.0/pycitysim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/utils/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/utils/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pycitysim/utils/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:35:26.540776 pycitysim-1.15.0/pycitysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-27 16:35:26.000000 pycitysim-1.15.0/pycitysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-27 16:35:26.000000 pycitysim-1.15.0/pycitysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:35:26.000000 pycitysim-1.15.0/pycitysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-27 16:35:26.000000 pycitysim-1.15.0/pycitysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 16:35:26.000000 pycitysim-1.15.0/pycitysim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-27 16:35:21.000000 pycitysim-1.15.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:35:26.540776 pycitysim-1.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 06:14:09.000000 pycitysim-1.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-30 06:14:19.840065 pycitysim-1.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 06:14:09.000000 pycitysim-1.15.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/apphub/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/apphub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/apphub/apphub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37841 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/map/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/routing/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/sateimg/
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sateimg/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sateimg/sateimg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.836065 pycitysim-1.15.1/pycitysim/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sidecar/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/pycitysim/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/aoi_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/clock_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/economy_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/lane_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/light_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/person_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/road_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/sim/social_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/pycitysim/streetview/
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/streetview/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/streetview/equirectangular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/streetview/google.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/pycitysim/urbankg/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/urbankg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/urbankg/kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/pycitysim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/utils/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/utils/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pycitysim/utils/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:14:19.840065 pycitysim-1.15.1/pycitysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-30 06:14:19.000000 pycitysim-1.15.1/pycitysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 06:14:19.000000 pycitysim-1.15.1/pycitysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:14:19.000000 pycitysim-1.15.1/pycitysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 06:14:19.000000 pycitysim-1.15.1/pycitysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 06:14:19.000000 pycitysim-1.15.1/pycitysim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-30 06:14:09.000000 pycitysim-1.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:14:19.844065 pycitysim-1.15.1/setup.cfg
```

### Comparing `pycitysim-1.15.0/LICENSE` & `pycitysim-1.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/PKG-INFO` & `pycitysim-1.15.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.15.0
+Version: 1.15.1
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.15.0/README.md` & `pycitysim-1.15.1/README.md`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/__init__.py` & `pycitysim-1.15.1/pycitysim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/apphub/apphub.py` & `pycitysim-1.15.1/pycitysim/apphub/apphub.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/map/map.py` & `pycitysim-1.15.1/pycitysim/map/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from geojson import Feature
 from google.protobuf.json_format import ParseDict
 from pycityproto.city.geo.v2 import geo_pb2
 from pycityproto.city.routing.v2 import routing_pb2
 from pycityproto.city.routing.v2 import routing_service_pb2 as routing_service
 from pymongo import MongoClient
 from shapely.geometry import LineString, Point, Polygon
-from shapely.ops import substring
+from shapely.ops import substring, unary_union
 
 __all__ = ["Map"]
 
 
 class Map:
     """
     模拟器地图API
@@ -65,14 +65,15 @@
 
         self.juncs: Dict[int, dict] = map_data["juncs"]
         """
         地图中的路口集合（junction），字典的值包含如下属性:
         The intersection collection (junction) in the map, the value of the dictionary contains the following attributes:
         - id (int): 路口编号。Junction ID.
         - lane_ids (list[int]): 属于该路口的所有车道和人行道编号。IDs of all driving and pedestrian lanes belonging to this junction.
+        - center (Dict[str, float]): 路口的大致中心点。The approximate center of the junction. example: {'x': 5983.14, 'y': 1807.73}
         """
 
         self.lanes: Dict[int, dict] = map_data["lanes"]
         """
         地图中的车道集合（lane），字典的值包含如下属性:
         The lane collection (lane) in the map. The value of the dictionary contains the following attributes:
         - id (int): 车道编号。Lane ID.
@@ -94,26 +95,23 @@
 
         self.roads: Dict[int, dict] = map_data["roads"]
         """
         地图中的道路集合（road），字典的值包含如下属性:
         The road collection (road) in the map, the value of the dictionary contains the following attributes:
         - id (int): 道路编号。Road ID.
         - lane_ids (list[int]): 道路所包含的车道和人行道编号。Driving and pedestrian lane IDs that the road contains.
-        - external["highway"] (string): OSM中的道路等级标签。Road class labels in OSM.
-        - external["name"] (string): 道路名称（不一定有）。Road name (not necessarily available).
         """
 
         self.aois: Dict[int, dict] = map_data["aois"]
         """
         地图中的AOI集合（aoi），字典的值包含如下属性:
         AOI collection (aoi) in the map, the value of the dictionary contains the following attributes:
         - id (int): AOI编号。AOI ID.
         - positions (list[XYPosition]): 多边形空间范围。Shape of polygon.
         - area (float): 面积(单位: m2)。Area.
-        - external["population"] (int): worldpop人口。population from WorldPop.
         - driving_positions (list[LanePosition]): 和道路网中行车道的连接点。Connection points to driving lanes.
         - walking_positions (list[LanePosition]): 和道路网中人行道的连接点。Connection points to pedestrian lanes.
         - driving_gates (list[XYPosition]): 和道路网中行车道的连接点对应的AOI边界上的位置。Position on the AOI boundary corresponding to the connection point to driving lanes.
         - walking_gates (list[XYPosition]): 和道路网中人行道的连接点对应的AOI边界上的位置。Position on the AOI boundary corresponding to the connection point to pedestrian lanes.
         - urban_land_use (Optional[str]): 城市建设用地分类，参照执行标准GB 50137-2011（https://www.planning.org.cn/law/uploads/2013/1383993139.pdf） Urban Land use type, refer to the national standard GB 50137-2011.
         - poi_ids (list[int]): 包含的POI列表。Contained POI IDs.
         - shapely_xy (shapely.geometry.Polygon): AOI的形状（xy坐标系）。Shape of polygon (in xy coordinates).
@@ -213,14 +211,22 @@
                 aoi["shapely_lnglat"] = Polygon(lnglat_positions)
         # 处理Poi的Geos
         for poi in pois.values():
             point = Point(poi["position"]["x"], poi["position"]["y"])
             poi["shapely_xy"] = point
             lng, lat = projector(point.x, point.y, inverse=True)
             poi["shapely_lnglat"] = Point([lng, lat])
+        # 为junction解算大致的中心点
+        for junc in juncs.values():
+            lane_shapelys = [
+                lanes[lane_id]["shapely_xy"] for lane_id in junc["lane_ids"]
+            ]
+            geos = unary_union(lane_shapelys)
+            center = geos.centroid
+            junc["center"] = {"x": center.x, "y": center.y}
 
         return {
             "header": header,
             "juncs": juncs,
             "roads": roads,
             "lanes": lanes,
             "aois": aois,
```

### Comparing `pycitysim-1.15.0/pycitysim/routing/client.py` & `pycitysim-1.15.1/pycitysim/routing/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sateimg/_utils.py` & `pycitysim-1.15.1/pycitysim/sateimg/_utils.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sateimg/sateimg.py` & `pycitysim-1.15.1/pycitysim/sateimg/sateimg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sidecar/sidecar.py` & `pycitysim-1.15.1/pycitysim/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/__init__.py` & `pycitysim-1.15.1/pycitysim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/aoi_service.py` & `pycitysim-1.15.1/pycitysim/sim/aoi_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/client.py` & `pycitysim-1.15.1/pycitysim/sim/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/clock_service.py` & `pycitysim-1.15.1/pycitysim/sim/clock_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/economy_services.py` & `pycitysim-1.15.1/pycitysim/sim/economy_services.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/event_service.py` & `pycitysim-1.15.1/pycitysim/sim/event_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/lane_service.py` & `pycitysim-1.15.1/pycitysim/sim/lane_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/light_service.py` & `pycitysim-1.15.1/pycitysim/sim/light_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/person_service.py` & `pycitysim-1.15.1/pycitysim/sim/person_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/road_service.py` & `pycitysim-1.15.1/pycitysim/sim/road_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/sim/social_service.py` & `pycitysim-1.15.1/pycitysim/sim/social_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/streetview/baidu.py` & `pycitysim-1.15.1/pycitysim/streetview/baidu.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/streetview/equirectangular.py` & `pycitysim-1.15.1/pycitysim/streetview/equirectangular.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/streetview/google.py` & `pycitysim-1.15.1/pycitysim/streetview/google.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/urbankg/kg.py` & `pycitysim-1.15.1/pycitysim/urbankg/kg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/utils/geojson.py` & `pycitysim-1.15.1/pycitysim/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/utils/grpc.py` & `pycitysim-1.15.1/pycitysim/utils/grpc.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim/utils/protobuf.py` & `pycitysim-1.15.1/pycitysim/utils/protobuf.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pycitysim.egg-info/PKG-INFO` & `pycitysim-1.15.1/pycitysim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.15.0
+Version: 1.15.1
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.15.0/pycitysim.egg-info/SOURCES.txt` & `pycitysim-1.15.1/pycitysim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycitysim-1.15.0/pyproject.toml` & `pycitysim-1.15.1/pyproject.toml`

 * *Files identical despite different names*

