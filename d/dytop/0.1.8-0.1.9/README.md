# Comparing `tmp/dytop-0.1.8.tar.gz` & `tmp/dytop-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dytop-0.1.8.tar", last modified: Thu May 30 14:29:15 2024, max compression
+gzip compressed data, was "dytop-0.1.9.tar", last modified: Thu May 30 14:44:45 2024, max compression
```

## Comparing `dytop-0.1.8.tar` & `dytop-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.532084 dytop-0.1.8/
--rw-r--r--   0 ewerton    (501) staff       (20)     1076 2023-09-20 01:44:57.000000 dytop-0.1.8/LICENSE
--rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:29:15.531330 dytop-0.1.8/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)      256 2024-05-30 14:20:44.000000 dytop-0.1.8/README.md
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.526872 dytop-0.1.8/dytop/
--rw-r--r--   0 ewerton    (501) staff       (20)     1412 2023-10-13 17:24:01.000000 dytop-0.1.8/dytop/Bistable_RoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)    17936 2023-10-13 17:23:52.000000 dytop-0.1.8/dytop/CMGDB_util.py
--rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-09-20 01:49:10.000000 dytop-0.1.8/dytop/Grid.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4441 2023-09-25 02:47:47.000000 dytop-0.1.8/dytop/Lips.py
--rw-r--r--   0 ewerton    (501) staff       (20)     1482 2024-05-29 20:04:42.000000 dytop-0.1.8/dytop/Morse_graph_updated.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4082 2024-05-29 20:04:40.000000 dytop-0.1.8/dytop/MultivaluedMap.py
--rw-r--r--   0 ewerton    (501) staff       (20)    11544 2024-01-13 01:33:10.000000 dytop-0.1.8/dytop/PlotRoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)     4722 2024-05-29 20:05:43.000000 dytop-0.1.8/dytop/Poset.py
--rw-r--r--   0 ewerton    (501) staff       (20)    10837 2024-05-29 20:04:44.000000 dytop-0.1.8/dytop/RoA.py
--rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-24 21:30:08.000000 dytop-0.1.8/dytop/__inity__.py
--rw-r--r--   0 ewerton    (501) staff       (20)      106 2023-10-02 02:22:07.000000 dytop-0.1.8/dytop/dyn_tools.py
-drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:29:15.530541 dytop-0.1.8/dytop.egg-info/
--rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/PKG-INFO
--rw-r--r--   0 ewerton    (501) staff       (20)      391 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/SOURCES.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        1 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/dependency_links.txt
--rw-r--r--   0 ewerton    (501) staff       (20)       49 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/requires.txt
--rw-r--r--   0 ewerton    (501) staff       (20)        6 2024-05-30 14:29:15.000000 dytop-0.1.8/dytop.egg-info/top_level.txt
--rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 03:41:35.000000 dytop-0.1.8/pyproject.toml
--rw-r--r--   0 ewerton    (501) staff       (20)       38 2024-05-30 14:29:15.532229 dytop-0.1.8/setup.cfg
--rw-r--r--   0 ewerton    (501) staff       (20)      480 2024-05-30 14:29:03.000000 dytop-0.1.8/setup.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:44:45.364633 dytop-0.1.9/
+-rw-r--r--   0 ewerton    (501) staff       (20)     1076 2023-09-20 01:44:57.000000 dytop-0.1.9/LICENSE
+-rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:44:45.363801 dytop-0.1.9/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)      256 2024-05-30 14:20:44.000000 dytop-0.1.9/README.md
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:44:45.358148 dytop-0.1.9/dytop/
+-rw-r--r--   0 ewerton    (501) staff       (20)     1412 2023-10-13 17:24:01.000000 dytop-0.1.9/dytop/Bistable_RoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    17936 2023-10-13 17:23:52.000000 dytop-0.1.9/dytop/CMGDB_util.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    12497 2023-09-20 01:49:10.000000 dytop-0.1.9/dytop/Grid.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4441 2023-09-25 02:47:47.000000 dytop-0.1.9/dytop/Lips.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     1482 2024-05-29 20:04:42.000000 dytop-0.1.9/dytop/Morse_graph_updated.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4082 2024-05-29 20:04:40.000000 dytop-0.1.9/dytop/MultivaluedMap.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    11544 2024-01-13 01:33:10.000000 dytop-0.1.9/dytop/PlotRoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)     4722 2024-05-29 20:05:43.000000 dytop-0.1.9/dytop/Poset.py
+-rw-r--r--   0 ewerton    (501) staff       (20)    10844 2024-05-30 14:44:12.000000 dytop-0.1.9/dytop/RoA.py
+-rw-r--r--   0 ewerton    (501) staff       (20)        0 2023-09-24 21:30:08.000000 dytop-0.1.9/dytop/__inity__.py
+-rw-r--r--   0 ewerton    (501) staff       (20)      106 2023-10-02 02:22:07.000000 dytop-0.1.9/dytop/dyn_tools.py
+drwxr-xr-x   0 ewerton    (501) staff       (20)        0 2024-05-30 14:44:45.363006 dytop-0.1.9/dytop.egg-info/
+-rw-r--r--   0 ewerton    (501) staff       (20)      644 2024-05-30 14:44:45.000000 dytop-0.1.9/dytop.egg-info/PKG-INFO
+-rw-r--r--   0 ewerton    (501) staff       (20)      391 2024-05-30 14:44:45.000000 dytop-0.1.9/dytop.egg-info/SOURCES.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        1 2024-05-30 14:44:45.000000 dytop-0.1.9/dytop.egg-info/dependency_links.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)       49 2024-05-30 14:44:45.000000 dytop-0.1.9/dytop.egg-info/requires.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)        6 2024-05-30 14:44:45.000000 dytop-0.1.9/dytop.egg-info/top_level.txt
+-rw-r--r--   0 ewerton    (501) staff       (20)      123 2023-10-13 03:41:35.000000 dytop-0.1.9/pyproject.toml
+-rw-r--r--   0 ewerton    (501) staff       (20)       38 2024-05-30 14:44:45.364781 dytop-0.1.9/setup.cfg
+-rw-r--r--   0 ewerton    (501) staff       (20)      480 2024-05-30 14:44:27.000000 dytop-0.1.9/setup.py
```

### Comparing `dytop-0.1.8/LICENSE` & `dytop-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/PKG-INFO` & `dytop-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dytop
-Version: 0.1.8
+Version: 0.1.9
 Summary: dytop: combinatorial DYnamics and TOPology
 Home-page: https://github.com/Ewerton-Vieira/dytop.git
 Author: Ewerton Rocha Vieira
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `dytop-0.1.8/dytop/Bistable_RoA.py` & `dytop-0.1.9/dytop/Bistable_RoA.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/CMGDB_util.py` & `dytop-0.1.9/dytop/CMGDB_util.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/Grid.py` & `dytop-0.1.9/dytop/Grid.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/Lips.py` & `dytop-0.1.9/dytop/Lips.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/Morse_graph_updated.py` & `dytop-0.1.9/dytop/Morse_graph_updated.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/MultivaluedMap.py` & `dytop-0.1.9/dytop/MultivaluedMap.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/PlotRoA.py` & `dytop-0.1.9/dytop/PlotRoA.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/Poset.py` & `dytop-0.1.9/dytop/Poset.py`

 * *Files identical despite different names*

### Comparing `dytop-0.1.8/dytop/RoA.py` & `dytop-0.1.9/dytop/RoA.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         # it is need to create the condensation graph
         for i in range(self.morse_graph.num_vertices()):
             for j in self.morse_graph.morse_set(i):
 
                 self.tiles_in_morse_sets[j] = i
 
         cyclic_Morse_graph = False
-        MG = .DirectedAcyclicGraph()  # building Morse Graph Poset
+        MG = pychomp.DirectedAcyclicGraph()  # building Morse Graph Poset
         MG.add_vertex(0)
         for u in range(morse_graph.num_vertices()):
             for v in morse_graph.adjacencies(u):
                 MG.add_edge(u, v)
                 if u in MG.adjacencies(v):  # prevent to compute with cyclic MG
                     cyclic_Morse_graph = True
```

### Comparing `dytop-0.1.8/dytop.egg-info/PKG-INFO` & `dytop-0.1.9/dytop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dytop
-Version: 0.1.8
+Version: 0.1.9
 Summary: dytop: combinatorial DYnamics and TOPology
 Home-page: https://github.com/Ewerton-Vieira/dytop.git
 Author: Ewerton Rocha Vieira
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
```

