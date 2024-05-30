# Comparing `tmp/brokerscore-0.1.2.tar.gz` & `tmp/brokerscore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brokerscore-0.1.2.tar", max compression
+gzip compressed data, was "brokerscore-0.1.3.tar", max compression
```

## Comparing `brokerscore-0.1.2.tar` & `brokerscore-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3630 2024-01-03 23:37:11.038721 brokerscore-0.1.2/README.md
--rw-r--r--   0        0        0      489 2024-01-12 22:29:40.722406 brokerscore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    19731 2024-01-12 22:29:27.577849 brokerscore-0.1.2/src/brokerscore.py
--rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 brokerscore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3630 2024-01-03 23:37:11.038721 brokerscore-0.1.3/README.md
+-rw-r--r--   0        0        0      489 2024-05-30 12:19:45.221280 brokerscore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    19877 2024-05-30 12:11:49.046484 brokerscore-0.1.3/src/brokerscore.py
+-rw-r--r--   0        0        0     4272 1970-01-01 00:00:00.000000 brokerscore-0.1.3/PKG-INFO
```

### Comparing `brokerscore-0.1.2/README.md` & `brokerscore-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `brokerscore-0.1.2/src/brokerscore.py` & `brokerscore-0.1.3/src/brokerscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         """
         nodes u and v are assumed to be neighbor nodes
         """
         return 1
 
 class iGraphConverter:
     """
-    Utility class to convert grpahs between formats,
+    Utility class to convert graphs between formats,
     baiscally Tulip and iGraph
     (used by the iGrpah implementation of the Leiden algorithm)
     """
 
     def __init__(self, tulip_graph):
         super(iGraphConverter, self).__init__()
         self.tulip_graph = tulip_graph
@@ -246,15 +246,19 @@
             gc = iGraphConverter(self.graph)
             iG = gc.to_igraph()
             communities = leidenalg.find_partition(
                 iG, leidenalg.ModularityVertexPartition
             )
             membership = communities.membership
             for n in self.graph.getNodes():
-                self.community[n] = membership[gc.node_to_index[n]]
+                try:
+                    self.community[n] = membership[gc.node_to_index[n]]
+                except TypeError:
+                    print('Node to index')
+                    print(gc.node_to_index)
 
     def collect_community_names(self):
         self.community_names = sorted(
             [sub.getName() for sub in self.graph.getSubGraphs()],
             key=lambda x: int(x.split("_")[1]),
         )
         self.nb_communities = len(self.community_names)
```

### Comparing `brokerscore-0.1.2/PKG-INFO` & `brokerscore-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brokerscore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Meso level network measure pbroker score as defined by Paquet-Clouston and Bouchard
 Author: Guy
 Author-email: guywiz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

