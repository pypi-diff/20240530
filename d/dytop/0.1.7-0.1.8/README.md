# Comparing `tmp/dytop-0.1.7.tar.gz` & `tmp/dytop-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dytop-0.1.7.tar", last modified: Fri Oct 13 17:50:25 2023, max compression
+gzip compressed data, was "dytop-0.1.8.tar", last modified: Thu May 30 14:29:15 2024, max compression
```

## Comparing `dytop-0.1.7.tar` & `dytop-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 17:50:25.771011 dytop-0.1.7/
--rw-r--r--   0 ewerton    (501) staff       (20)     1076 2023-09-20 01:44:57.000000 dytop-0.1.7/LICENSE
--rw-r--r--   0 ewerton    (501) staff       (20)      496 2023-10-13 17:50:25.770466 dytop-0.1.7/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)      148 2023-09-25 02:45:17.000000 dytop-0.1.7/README.md
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 17:50:25.766904 dytop-0.1.7/dytop/
--rw-r--r--   0 ewerton    (501) staff       (20)     1412 2023-10-13 17:24:01.000000 dytop-0.1.7/dytop/Bistable_RoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)    17936 2023-10-13 17:23:52.000000 dytop-0.1.7/dytop/CMGDB_util.py
--rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-09-20 01:49:10.000000 dytop-0.1.7/dytop/Grid.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4441 2023-09-25 02:47:47.000000 dytop-0.1.7/dytop/Lips.py
--rw-r--r--   0 ewerton    (501) staff       (20)     1483 2023-09-25 02:46:45.000000 dytop-0.1.7/dytop/Morse_graph_updated.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4086 2023-09-25 00:30:11.000000 dytop-0.1.7/dytop/MultivaluedMap.py
--rw-r--r--   0 ewerton    (501) staff       (20)    11537 2023-09-25 02:46:44.000000 dytop-0.1.7/dytop/PlotRoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4723 2023-09-20 15:51:13.000000 dytop-0.1.7/dytop/Poset.py
--rw-r--r--   0 ewerton    (501) staff       (20)    10608 2023-10-13 17:25:05.000000 dytop-0.1.7/dytop/RoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-24 21:30:08.000000 dytop-0.1.7/dytop/__inity__.py
--rw-r--r--   0 ewerton    (501) staff       (20)      106 2023-10-02 02:22:07.000000 dytop-0.1.7/dytop/dyn_tools.py
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2023-10-13 17:50:25.769814 dytop-0.1.7/dytop.egg-info/
--rw-r--r--   0 ewerton    (501) staff       (20)      496 2023-10-13 17:50:25.000000 dytop-0.1.7/dytop.egg-info/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)      391 2023-10-13 17:50:25.000000 dytop-0.1.7/dytop.egg-info/SOURCES.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        1 2023-10-13 17:50:25.000000 dytop-0.1.7/dytop.egg-info/dependency_links.txt
--rw-r--r--   0 ewerton    (501) staff       (20)       49 2023-10-13 17:50:25.000000 dytop-0.1.7/dytop.egg-info/requires.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        6 2023-10-13 17:50:25.000000 dytop-0.1.7/dytop.egg-info/top_level.txt
--rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 03:41:35.000000 dytop-0.1.7/pyproject.toml
--rw-r--r--   0 ewerton    (501) staff       (20)       38 2023-10-13 17:50:25.771114 dytop-0.1.7/setup.cfg
--rw-r--r--   0 ewerton    (501) staff       (20)      429 2023-10-13 17:49:56.000000 dytop-0.1.7/setup.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.532084 dytop-0.1.8/
+-rw-r--r--   0 ewerton    (501) staff       (20)     1076 2023-09-20 01:44:57.000000 dytop-0.1.8/LICENSE
+-rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:29:15.531330 dytop-0.1.8/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)      256 2024-05-30 14:20:44.000000 dytop-0.1.8/README.md
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.526872 dytop-0.1.8/dytop/
+-rw-r--r--   0 ewerton    (501) staff       (20)     1412 2023-10-13 17:24:01.000000 dytop-0.1.8/dytop/Bistable_RoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    17936 2023-10-13 17:23:52.000000 dytop-0.1.8/dytop/CMGDB_util.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-09-20 01:49:10.000000 dytop-0.1.8/dytop/Grid.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4441 2023-09-25 02:47:47.000000 dytop-0.1.8/dytop/Lips.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     1482 2024-05-29 20:04:42.000000 dytop-0.1.8/dytop/Morse_graph_updated.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4082 2024-05-29 20:04:40.000000 dytop-0.1.8/dytop/MultivaluedMap.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    11544 2024-01-13 01:33:10.000000 dytop-0.1.8/dytop/PlotRoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4722 2024-05-29 20:05:43.000000 dytop-0.1.8/dytop/Poset.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    10837 2024-05-29 20:04:44.000000 dytop-0.1.8/dytop/RoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-24 21:30:08.000000 dytop-0.1.8/dytop/__inity__.py
+-rw-r--r--   0 ewerton    (501) staff       (20)      106 2023-10-02 02:22:07.000000 dytop-0.1.8/dytop/dyn_tools.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.530541 dytop-0.1.8/dytop.egg-info/
+-rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)      391 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/SOURCES.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        1 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/dependency_links.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)       49 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/requires.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        6 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/top_level.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 03:41:35.000000 dytop-0.1.8/pyproject.toml
+-rw-r--r--   0 ewerton    (501) staff       (20)       38 2024-05-30 14:29:15.532229 dytop-0.1.8/setup.cfg
+-rw-r--r--   0 ewerton    (501) staff       (20)      480 2024-05-30 14:29:03.000000 dytop-0.1.8/setup.py
```

### Comparing `dytop-0.1.7/LICENSE` & `dytop-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dytop-0.1.7/dytop/Bistable_RoA.py` & `dytop-0.1.8/dytop/Bistable_RoA.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.7/dytop/CMGDB_util.py` & `dytop-0.1.8/dytop/CMGDB_util.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.7/dytop/Grid.py` & `dytop-0.1.8/dytop/Grid.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.7/dytop/Lips.py` & `dytop-0.1.8/dytop/Lips.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.7/dytop/Morse_graph_updated.py` & `dytop-0.1.8/dytop/Morse_graph_updated.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Morse_graph_updated:
     def __init__(self, morse_graph, MG_updated):
 
         self.morse_graph = morse_graph
 
         self.MG_ = Poset.Poset(MG_updated)
 
-        self.MG_updated_ = pychomp2.DirectedAcyclicGraph()  # building Morse Graph Poset
+        self.MG_updated_ = pychomp.DirectedAcyclicGraph()  # building Morse Graph Poset
         self.MG_updated_.add_vertex(0)
 
         for u in self.morse_graph.vertices():
             for v in self.MG_.parents(u):
                 self.MG_updated_.add_edge(v, u)  # inverse since RoA build MG_updated inverted
 
         # for (u,v) in self.morse_graph.edges():
```

### Comparing `dytop-0.1.7/dytop/MultivaluedMap.py` & `dytop-0.1.8/dytop/MultivaluedMap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MultivaluedMap.py  # 2021-20-10
 # MIT LICENSE 2020 Ewerton R. Vieira
-import pychomp2
+import pychomp
 import graphviz
 import dytop.Poset as Poset
 
 
 def Dict_inverse(D):
     """Return the inverse of a dictionary D"""
     inv_map = {}
@@ -29,28 +29,28 @@
         num_verts = map_graph.num_vertices()
 
         self.vertices_ = {a for a in range(num_verts)}
 
         self.map_graph = map_graph
 
         # self.mapping: map_graph -> condensation_graph
-        condensation_graph, self.mapping = pychomp2.CondensationGraph(
+        condensation_graph, self.mapping = pychomp.CondensationGraph(
             self.vertices_, map_graph.adjacencies)
 
         self.CG = condensation_graph
         # self.CG.graphviz = self.condensation_graph_with_labels
 
         self.mapping_inv = {}  # inverse of mapping condensation_graph -> map_graph
         for key, value in self.mapping.items():
             self.mapping_inv.setdefault(value, []).append(key)
 
         # condensation_graph with poset structure
         self.condensation_graph = Poset.Poset(condensation_graph, save_memory=True)
 
-        MG = pychomp2.DirectedAcyclicGraph()  # building Morse Graph Poset
+        MG = pychomp.DirectedAcyclicGraph()  # building Morse Graph Poset
         MG.add_vertex(0)
         for u in range(morse_graph.num_vertices()):
             for v in morse_graph.adjacencies(u):
                 MG.add_edge(u, v)
         self.MG = Poset.Poset(MG)
 
     def vertices(self):
@@ -65,15 +65,15 @@
         """
         U = []
         for a in self.condensation_graph.ancestors(self.mapping[v]).union({self.mapping[v]}):
             U = U + self.mapping_inv[a]
         return set(U)
 
     def mvm_graph(self):
-        mvm = pychomp2.DirectedAcyclicGraph()  # building domain graph
+        mvm = pychomp.DirectedAcyclicGraph()  # building domain graph
         mvm.add_vertex(0)
         for v in self.vertices():
             for u in self.map_graph.adjacencies(v):
                 mvm.add_edge(v, u)
         return mvm
 
     def build_viz(self, graph, shape='circle'):
```

### Comparing `dytop-0.1.7/dytop/PlotRoA.py` & `dytop-0.1.8/dytop/PlotRoA.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     if from_file and not from_file_basic:
 
         # read file
         from_file = dir_path + from_file + "_RoA_" + ".csv"
         with open(from_file, "r") as file:
             f = csv.reader(file, delimiter=',')
             next(f)
-            box_size = [float(i) for i in next(f)]
+            box_size = [float(i) for i in next(f)[0:dim]]
             next(f)
             Tiles = []
             Morse_nodes = []
             Boxes = []
             num_morse_sets = 0
             counter_temp = 0
             for row in f:
```

### Comparing `dytop-0.1.7/dytop/Poset.py` & `dytop-0.1.8/dytop/Poset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Poset.py  # 2021-20-10
 # Base on Shaun Poset.py
 # MIT LICENSE 2020 Ewerton R. Vieira
 
-from pychomp2.DirectedAcyclicGraph import *
+from pychomp.DirectedAcyclicGraph import *
 import graphviz
 
 
 class Poset:  # Represent a Poset
 
     def ListOfNivelSets(self):  # return the list of increasing Nivel sets of a given poset
```

### Comparing `dytop-0.1.7/dytop/RoA.py` & `dytop-0.1.8/dytop/RoA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # RoA.py  # 2022-20-01
 # MIT LICENSE 2020 Ewerton R. Vieira
 
-import pychomp2
+import pychomp
 import CMGDB
 
 import numpy as np
 import csv
 import os
 
 import matplotlib
@@ -51,15 +51,15 @@
         return morse_node
 
     def assign_morse_nodes2tiles_adaptive(self):
         """For each tile assign a morse node (creating a region of attraction for a downset)
          Inclui adaptive grid"""
 
         # It will create a updated Morse graph
-        self.MG_updated = pychomp2.DirectedAcyclicGraph()
+        self.MG_updated = pychomp.DirectedAcyclicGraph()
         for vertice in range(self.morse_graph.num_vertices()):
             self.MG_updated.add_vertex(vertice)
 
 
         # clone self.tiles_in_morse_sets we dont have to recompute
         self.dict_tiles = dict(self.tiles_in_morse_sets)
 
@@ -144,15 +144,15 @@
         # it is need to create the condensation graph
         for i in range(self.morse_graph.num_vertices()):
             for j in self.morse_graph.morse_set(i):
 
                 self.tiles_in_morse_sets[j] = i
 
         cyclic_Morse_graph = False
-        MG = pychomp2.DirectedAcyclicGraph()  # building Morse Graph Poset
+        MG = .DirectedAcyclicGraph()  # building Morse Graph Poset
         MG.add_vertex(0)
         for u in range(morse_graph.num_vertices()):
             for v in morse_graph.adjacencies(u):
                 MG.add_edge(u, v)
                 if u in MG.adjacencies(v):  # prevent to compute with cyclic MG
                     cyclic_Morse_graph = True
 
@@ -195,19 +195,24 @@
         return [rect[i] + (rect[dim + i] - rect[i])/2 for i in range(dim)]
 
     def save_file(self, name=""):
         rect = self.morse_graph.phase_space_box(0)
         dim = int(len(rect) // 2)
         size_box = [rect[dim + i] - rect[i] for i in range(dim)]
 
+        # getting the bounds
+        lower_bounds = rect[0:dim]
+        rect = self.morse_graph.phase_space_box(self.map_graph.num_vertices()-1)
+        upper_bounds = rect[dim::]
+
         name = self.dir_path + name + "_RoA_" + ".csv"
         with open(name, "w") as file:
             f = csv.writer(file)
-            f.writerow(["Box size"])
-            f.writerow(size_box)
+            f.writerow(["Box size", "Lower bounds", "Upper bounds"])
+            f.writerow(size_box+lower_bounds+upper_bounds)
             f.writerow(["Tile", "Morse_node", "Box"])
 
             if self.dict_tiles:  # it might be empty
                 # tiles in roa
                 for tile_in_roa in set(self.dict_tiles.items()) - set(self.tiles_in_morse_sets.items()):
                     tile_in_roa = list(tile_in_roa) + \
                         [a for a in self.morse_graph.phase_space_box(tile_in_roa[0])]
```

