# Comparing `tmp/mummichog-2.6.1.tar.gz` & `tmp/mummichog-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shuzhao/li.github/mummichog/dist/tmpqs150rm9/mummichog-2.6.1.tar", last modified: Mon Feb  7 22:13:19 2022, max compression
+gzip compressed data, was "mummichog-2.7.0.tar", last modified: Thu May 30 01:57:29 2024, max compression
```

## Comparing `mummichog-2.6.1.tar` & `mummichog-2.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2022-02-07 22:13:19.000000 mummichog-2.6.1/
--rwxr-xr-x   0 shuzhao    (501) staff       (20)      360 2020-08-12 02:17:06.000000 mummichog-2.6.1/LICENSE
--rw-r--r--   0 shuzhao    (501) staff       (20)     3283 2022-02-07 22:13:19.000000 mummichog-2.6.1/PKG-INFO
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     2346 2022-02-07 16:01:50.000000 mummichog-2.6.1/README.md
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog/
--rwxr-xr-x   0 shuzhao    (501) staff       (20)  6803492 2022-02-06 15:12:02.000000 mummichog-2.6.1/mummichog/JSON_metabolicModels.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2020-03-12 13:48:32.000000 mummichog-2.6.1/mummichog/__init__.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)       29 2020-08-12 02:17:06.000000 mummichog-2.6.1/mummichog/command_line.py
--rw-r--r--   0 shuzhao    (501) staff       (20)  5094183 2022-02-06 23:54:26.000000 mummichog-2.6.1/mummichog/compound_dicts.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    10070 2022-02-07 02:06:14.000000 mummichog-2.6.1/mummichog/config.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)  9277661 2022-02-06 14:57:35.000000 mummichog-2.6.1/mummichog/cp__JSON_metabolicModels.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    25781 2020-08-12 02:17:06.000000 mummichog-2.6.1/mummichog/functional_analysis.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    31112 2022-02-06 23:42:34.000000 mummichog-2.6.1/mummichog/get_user_data.py
--rw-r--r--   0 shuzhao    (501) staff       (20)     4349 2022-02-06 15:25:49.000000 mummichog-2.6.1/mummichog/ions.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     3240 2022-02-07 01:10:19.000000 mummichog-2.6.1/mummichog/main.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    14604 2022-02-07 02:04:31.000000 mummichog-2.6.1/mummichog/models.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    16448 2020-03-12 13:48:32.000000 mummichog-2.6.1/mummichog/ng_modularity.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)    33974 2022-02-07 02:04:31.000000 mummichog-2.6.1/mummichog/reporting.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog/resources/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2020-10-19 23:15:25.000000 mummichog-2.6.1/mummichog/resources/__init__.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     5409 2020-08-12 02:17:06.000000 mummichog-2.6.1/mummichog/resources/plotly-graphs.js
--rwxr-xr-x   0 shuzhao    (501) staff       (20)  3311389 2020-08-12 02:17:06.000000 mummichog-2.6.1/mummichog/resources/plotly-latest.min.js
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog/tests/
--rw-r--r--   0 shuzhao    (501) staff       (20)        0 2020-10-19 23:15:25.000000 mummichog-2.6.1/mummichog/tests/__init__.py
--rwxr-xr-x   0 shuzhao    (501) staff       (20)   419112 2020-03-12 13:48:32.000000 mummichog-2.6.1/mummichog/tests/testdata0710.txt
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     8877 2020-08-12 02:17:06.000000 mummichog-2.6.1/mummichog/websnippets.py
-drwxr-xr-x   0 shuzhao    (501) staff       (20)        0 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/
--rw-r--r--   0 shuzhao    (501) staff       (20)     3283 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/PKG-INFO
--rw-r--r--   0 shuzhao    (501) staff       (20)      784 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/SOURCES.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/dependency_links.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       59 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/entry_points.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       49 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/requires.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)       10 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/top_level.txt
--rw-r--r--   0 shuzhao    (501) staff       (20)        1 2022-02-07 22:13:19.000000 mummichog-2.6.1/mummichog.egg-info/zip-safe
--rw-r--r--   0 shuzhao    (501) staff       (20)       38 2022-02-07 22:13:19.000000 mummichog-2.6.1/setup.cfg
--rwxr-xr-x   0 shuzhao    (501) staff       (20)     1597 2022-02-07 02:05:58.000000 mummichog-2.6.1/setup.py
+drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-05-30 01:57:29.529448 mummichog-2.7.0/
+-rwxr-xr-x   0 lish     (195676001) 1088672553      360 2024-02-02 16:25:50.000000 mummichog-2.7.0/LICENSE
+-rw-r--r--   0 lish     (195676001) 1088672553     3384 2024-05-30 01:57:29.529016 mummichog-2.7.0/PKG-INFO
+-rwxr-xr-x   0 lish     (195676001) 1088672553     2346 2024-02-02 16:25:50.000000 mummichog-2.7.0/README.md
+drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-05-30 01:57:29.519973 mummichog-2.7.0/mummichog/
+-rwxr-xr-x   0 lish     (195676001) 1088672553  6803492 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/JSON_metabolicModels.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/__init__.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553       29 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/command_line.py
+-rw-r--r--   0 lish     (195676001) 1088672553  5094183 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/compound_dicts.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    10070 2024-05-30 01:51:31.000000 mummichog-2.7.0/mummichog/config.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    26237 2024-05-30 01:42:58.000000 mummichog-2.7.0/mummichog/functional_analysis.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    31112 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/get_user_data.py
+-rw-r--r--   0 lish     (195676001) 1088672553     4349 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/ions.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553     3240 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/main.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    14632 2024-05-30 01:47:02.000000 mummichog-2.7.0/mummichog/models.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    16637 2024-05-30 01:55:31.000000 mummichog-2.7.0/mummichog/ng_modularity.py
+-rw-r--r--   0 lish     (195676001) 1088672553      529 2024-05-30 01:41:21.000000 mummichog-2.7.0/mummichog/nx_modularity.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553    33990 2024-05-30 01:50:39.000000 mummichog-2.7.0/mummichog/reporting.py
+drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-05-30 01:57:29.524324 mummichog-2.7.0/mummichog/resources/
+-rw-r--r--   0 lish     (195676001) 1088672553        0 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/resources/__init__.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553     5409 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/resources/plotly-graphs.js
+-rwxr-xr-x   0 lish     (195676001) 1088672553  3311389 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/resources/plotly-latest.min.js
+drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-05-30 01:57:29.527478 mummichog-2.7.0/mummichog/tests/
+-rw-r--r--   0 lish     (195676001) 1088672553        0 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/tests/__init__.py
+-rwxr-xr-x   0 lish     (195676001) 1088672553   419112 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/tests/testdata0710.txt
+-rwxr-xr-x   0 lish     (195676001) 1088672553     8877 2024-02-02 16:25:50.000000 mummichog-2.7.0/mummichog/websnippets.py
+drwxr-xr-x   0 lish     (195676001) 1088672553        0 2024-05-30 01:57:29.528406 mummichog-2.7.0/mummichog.egg-info/
+-rw-r--r--   0 lish     (195676001) 1088672553     3384 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/PKG-INFO
+-rw-r--r--   0 lish     (195676001) 1088672553      773 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/SOURCES.txt
+-rw-r--r--   0 lish     (195676001) 1088672553        1 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/dependency_links.txt
+-rw-r--r--   0 lish     (195676001) 1088672553       58 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/entry_points.txt
+-rw-r--r--   0 lish     (195676001) 1088672553       46 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/requires.txt
+-rw-r--r--   0 lish     (195676001) 1088672553       10 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/top_level.txt
+-rw-r--r--   0 lish     (195676001) 1088672553        1 2024-05-30 01:57:29.000000 mummichog-2.7.0/mummichog.egg-info/zip-safe
+-rw-r--r--   0 lish     (195676001) 1088672553       38 2024-05-30 01:57:29.529495 mummichog-2.7.0/setup.cfg
+-rwxr-xr-x   0 lish     (195676001) 1088672553     1594 2024-05-30 00:56:21.000000 mummichog-2.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mummichog-2.6.1/PKG-INFO` & `mummichog-2.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: mummichog
-Version: 2.6.1
+Version: 2.7.0
 Summary: Pathway and network analysis for metabolomics data
 Home-page: https://github.com/shuzhao-li/mummichog
 Author: Shuzhao Li, Francisco Castellanos, Andrei Todor
 Author-email: shuzhao.li@gmail.com
 License: BSD 3-Clause
 Keywords: metabolomics analysis bioinformatics mass spectrometry systems biology
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: networkx>=2
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: xlsxwriter
 
 Mummichog
 =========
 
 Mummichog is a Python program for analyzing data from high throughput, untargeted metabolomics.
 It leverages the organization of metabolic networks to predict functional activity directly from feature tables,
 bypassing metabolite identification. The features include
@@ -73,9 +77,7 @@
 *Python 3 is required for Mummichog version 2.3 and beyond.*
 
 *Mummichog version 2.2 was the last version using Python 2; new branch as mummichog-python2*
 
 The initial paper on mummichog is described in Li et al. Predicting Network Activity from High Throughput Metabolomics. PLoS Computational Biology (2013); doi:10.1371/journal.pcbi.1003123. 
 
 More on [project website http://mummichog.org](http://mummichog.org).
-
-
```

### Comparing `mummichog-2.6.1/README.md` & `mummichog-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/JSON_metabolicModels.py` & `mummichog-2.7.0/mummichog/JSON_metabolicModels.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/compound_dicts.py` & `mummichog-2.7.0/mummichog/compound_dicts.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/config.py` & `mummichog-2.7.0/mummichog/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 '''
 configuration and utility functions of mummichog
 
 To move adduct calculation out to azimuth-metabolomics.
 
 '''
 
-VERSION = '2.6.1'          # Python 3 only
+VERSION = '2.7.0'          # Python 3 only
 RELEASE = True
 USE_DEBUG = False
 
 
 import sys
 import os
 import inspect
```

### Comparing `mummichog-2.6.1/mummichog/functional_analysis.py` & `mummichog-2.7.0/mummichog/functional_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 '''
 
 import logging
 import random
 import itertools
 
 from scipy import stats
-import mummichog.ng_modularity as NGM
+import mummichog.nx_modularity as NGM
 
 from .get_user_data import *
 
 
 logging.basicConfig(format='%(message)s', level=logging.INFO)
 
 
@@ -435,15 +435,17 @@
                 new_network = nx.from_edgelist(edges)
                 
             else:
                 # step 1, 2, 3, ... growing to include extra steps/connections
                 new_network = nx.from_edgelist(edges)
                 seeds = new_network.nodes()
             
-            for sub in nx.connected_component_subgraphs(new_network):
+            # for sub in nx.connected_component_subgraphs(new_network):
+            for sub in nx.connected_components(new_network):
+                sub = new_network.subgraph(sub).copy()
                 if 3 < sub.number_of_nodes() < MODULE_SIZE_LIMIT:
                     M = Mmodule(self.network, sub, TrioList)
                     modules.append(M)
                 
         # add modules split from modules
         if USE_DEBUG:
             logging.info( '# initialized network size = %d' %len(seeds) )
@@ -477,27 +479,36 @@
         
     def __split_modules__(self, g):
         '''
         return nx.graph instance after splitting the input graph
         by Newman's spectral split method
         Only modules more than 3 nodes are considered as good small modules 
         should have been generated in 1st connecting step.
-        '''
+        
         net = NGM.network()
         net.copy_from_graph(g)
         return [nx.subgraph(g, x) for x in net.specsplit() if len(x) > 3]
+    
+        '''
+        return [nx.subgraph(g, x) for x in NGM.find_communities(g) if len(x) > 3]
+    
+
+    
 
     # test alternative algorithm
     def __split_modules_nemo__(self, g):
         '''
         Alternative function using NeMo algorithm for module finding.
+        
         Not used for now.
-        '''
+        
         net = NGM.nemo_network(g)
         return [nx.subgraph(g, x) for x in net.find_modules() if len(x) > 3]
+        '''
+        pass
 
 
     def rank_significance(self):
         '''
         compute p-values of modules. Either model based:
         scores of random modules are fitted to a Gamma distribution,
         p-value is calculated from CDF.
@@ -651,16 +662,22 @@
         out = open(filename, 'w')
         out.write(s)
         out.close()
         
     def __get_largest_subgraph__(self, an):
         '''
         connected_component_subgraphs likely to return sorted subgraphs. Just to be sure here.
+        
+                    for sub in nx.connected_components(new_network):
+                sub = new_network.subgraph(sub).copy()
+                
         '''
-        return max(nx.connected_component_subgraphs(an), key=len)
+        return max(
+            [an.subgraph(c).copy() for c in nx.connected_components(an)], key=len
+            )
         
     def __get_ave_connections__(self, N):
         '''
         nx.average_node_connectivity(G) is too slow; use self.__get_ave_connections__()
         '''
         try:                #Avoid ZeroDivisionError
             return N.number_of_edges()/float(N.number_of_nodes())
```

### Comparing `mummichog-2.6.1/mummichog/get_user_data.py` & `mummichog-2.7.0/mummichog/get_user_data.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/ions.py` & `mummichog-2.7.0/mummichog/ions.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/main.py` & `mummichog-2.7.0/mummichog/main.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/models.py` & `mummichog-2.7.0/mummichog/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         to keep tracking of where the EmpCpd came from (mzFeature).
         
         network is the total parent metabolic network
         '''
         self.network = network
         self.num_ref_edges = self.network.number_of_edges()
         self.num_ref_nodes = self.network.number_of_nodes()
-        self.graph = subgraph
+        self.graph = subgraph.copy()
         
         seed_cpds = [x[2] for x in TrioList]
         self.shave(seed_cpds)
         self.nodestr = self.make_nodestr()
         self.N_seeds = len(seed_cpds)
         self.A = self.activity_score(seed_cpds, self.get_num_EmpCpd(TrioList))
     
@@ -342,24 +342,25 @@
         '''
         shave off nodes that do not connect seeds, i.e.
         any node with degree = 1 and is not a seed, iteratively.
         '''
         nonseeds = [x for x in self.graph.nodes() if x not in seed_cpds]
         excessive = [x for x in nonseeds if self.graph.degree(x)==1]
         while excessive:
-            for x in excessive: self.graph.remove_node(x)
+            for x in excessive: 
+                self.graph.remove_node(x)
             nonseeds = [x for x in self.graph.nodes() if x not in seed_cpds]
             excessive = [x for x in nonseeds if self.graph.degree(x)==1]
 
 
     def make_nodestr(self):
         '''
         create an identifier using nodes in sorted order
         '''
-        Nodes = self.graph.nodes()
+        Nodes = list(self.graph.nodes)
         Nodes.sort()
         return ''.join(Nodes)
 
     def export_network_txt(self, met_model, filename):
         '''
         To use .txt for Cytoscape 3, no need for .sif any more.
         Edges are strings now as switching to JSON compatible.
```

### Comparing `mummichog-2.6.1/mummichog/ng_modularity.py` & `mummichog-2.7.0/mummichog/ng_modularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 
 This was from Ca. 2008... 
 Future work should improve its efficiency or use a more efficient module-finding algorithm.
 Modified to add fielding numpy.linalg.linalg.linAlgError, Shuzhao Li, 2017-05-15
 Modified to fit Python 3, 2020-02-12
 """
 
+
+#
+# Deprecated; too many changes btw networkx v1 and v2. Use nx_modularity instead
+#
+
 USE_TEST_MODE = False
 
+import networkx as nx
 from numpy import *
 
 if USE_TEST_MODE:
     import re, itertools
-    import networkx as nx
     from scipy.cluster import hierarchy
 
 
 class module:
     """
     A mudule is a list of nodes within a reference network.
     self.divide(nobj) returns delta_Q and [group1, group2].
@@ -215,28 +220,32 @@
             print ("Degrees already exist!")
 
     def make_adjacency_matrix(self):
         """
         Make adjacency matrix from nodes and edges.
         Edges are treated as not directional, thus matrix is symmetrical.
         Multiple edges between two nodes are allowed.
-        """
+        
         am = zeros( (self.num_nodes, self.num_nodes) )
         for edge in self.edges:
             am[self.nodes.index(edge[0]), self.nodes.index(edge[1])] += 1
             # take out the next line will make a directional network
             am[self.nodes.index(edge[1]), self.nodes.index(edge[0])] += 1
         self.adjacency_matrix = am
+        
+        """
+        self.adjacency_matrix = nx.adjacency_matrix(self)
 
     def make_node_index(self):
         """
         mapping node name/id to original index
         """
+        nodes = list(self.nodes)
         for ii in range(self.num_nodes):
-            self.crd[self.nodes[ii]] = ii
+            self.crd[ nodes[ii] ] = ii
 
     #
     # The read_gml functions read network from GML format.
     # Alternatively, self.nodes and self.edges can be directly defined.
     #
 
     def copy_from_graph(self, g):
```

### Comparing `mummichog-2.6.1/mummichog/reporting.py` & `mummichog-2.7.0/mummichog/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         AN yet to be revised
         
         '''
         self.web_export_networks = [M.graph for M in self.MA.top_modules[:5]] + [self.AN.activity_network]
         
         
         vis_nodes = []
-        for g in self.web_export_networks: vis_nodes += g.nodes()
+        for g in self.web_export_networks: vis_nodes += list(g.nodes)
         self.vis_nodes = set(vis_nodes)
 
 
     def web_export(self):
         '''
         Return HTML without head/foot.
         '''
@@ -211,15 +211,15 @@
             M.export_network_txt(self.model, 
                                  os.path.join(self.moduledir, 'module_' + str(counter) + '.txt'))
         
         '''
         s, counter = '', 0
         for M in self.MA.top_modules:
             counter += 1
-            nodes = M.graph.nodes()
+            nodes = list(M.graph.nodes)
             names = [self.model.dict_cpds_def.get(x, '') for x in nodes]
             s += '<div class="moduleline">' + 'module_' + str(counter) + ", p=" + str(round(M.p_value, 5)) + ", " + str(len(nodes)) + " metabolites" + '</div>'
             s += '<div class="metabolites">' + ', '.join(names) + '</div>'
             
         return s + '\n'
 
 
@@ -410,15 +410,15 @@
         Write .tsv report for top modules.
         '''
         resultstr = [
                      ['MODULE', 'p-value', 'size', 'members (name)', 'members (id)', 
                       'This module overlaps with'], ]
         
         for M in self.MA.top_modules:
-            nodes = M.graph.nodes()
+            nodes = list(M.graph.nodes)
             names = [self.model.dict_cpds_def.get(x, '') for x in nodes]
             resultstr.append([M.id, str(M.p_value),
                               str(len(nodes)), '$'.join(names),
                               ','.join(nodes), self.find_top_pathways(nodes),
                                ])
 
         outfile = os.path.join(self.tabledir, "mcg_modularanalysis_") + self.data.paradict['output']
@@ -576,15 +576,15 @@
                 } for P in self.PA.resultListOfPathways
             ],
 
             'result_networkModules' : [
                 {
                     'id': M.id,
                     'p_value': M.p_value,
-                    'members': M.graph.nodes(), # This is on theoretical metabolites/compounds
+                    'members': list(M.graph.nodes), # This is on theoretical metabolites/compounds
                     #'size' is number of members
                     # Common names of members can be looked up, from metabolic model/metabolite definition
                 } for M in self.MA.top_modules
             ],
 
         }
```

### Comparing `mummichog-2.6.1/mummichog/resources/plotly-graphs.js` & `mummichog-2.7.0/mummichog/resources/plotly-graphs.js`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/resources/plotly-latest.min.js` & `mummichog-2.7.0/mummichog/resources/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/tests/testdata0710.txt` & `mummichog-2.7.0/mummichog/tests/testdata0710.txt`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog/websnippets.py` & `mummichog-2.7.0/mummichog/websnippets.py`

 * *Files identical despite different names*

### Comparing `mummichog-2.6.1/mummichog.egg-info/PKG-INFO` & `mummichog-2.7.0/mummichog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: mummichog
-Version: 2.6.1
+Version: 2.7.0
 Summary: Pathway and network analysis for metabolomics data
 Home-page: https://github.com/shuzhao-li/mummichog
 Author: Shuzhao Li, Francisco Castellanos, Andrei Todor
 Author-email: shuzhao.li@gmail.com
 License: BSD 3-Clause
 Keywords: metabolomics analysis bioinformatics mass spectrometry systems biology
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: networkx>=2
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: xlsxwriter
 
 Mummichog
 =========
 
 Mummichog is a Python program for analyzing data from high throughput, untargeted metabolomics.
 It leverages the organization of metabolic networks to predict functional activity directly from feature tables,
 bypassing metabolite identification. The features include
@@ -73,9 +77,7 @@
 *Python 3 is required for Mummichog version 2.3 and beyond.*
 
 *Mummichog version 2.2 was the last version using Python 2; new branch as mummichog-python2*
 
 The initial paper on mummichog is described in Li et al. Predicting Network Activity from High Throughput Metabolomics. PLoS Computational Biology (2013); doi:10.1371/journal.pcbi.1003123. 
 
 More on [project website http://mummichog.org](http://mummichog.org).
-
-
```

### Comparing `mummichog-2.6.1/mummichog.egg-info/SOURCES.txt` & `mummichog-2.7.0/mummichog.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 README.md
 setup.py
 mummichog/JSON_metabolicModels.py
 mummichog/__init__.py
 mummichog/command_line.py
 mummichog/compound_dicts.py
 mummichog/config.py
-mummichog/cp__JSON_metabolicModels.py
 mummichog/functional_analysis.py
 mummichog/get_user_data.py
 mummichog/ions.py
 mummichog/main.py
 mummichog/models.py
 mummichog/ng_modularity.py
+mummichog/nx_modularity.py
 mummichog/reporting.py
 mummichog/websnippets.py
 mummichog.egg-info/PKG-INFO
 mummichog.egg-info/SOURCES.txt
 mummichog.egg-info/dependency_links.txt
 mummichog.egg-info/entry_points.txt
 mummichog.egg-info/requires.txt
```

### Comparing `mummichog-2.6.1/setup.py` & `mummichog-2.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
   name='mummichog',
-  version='2.6.1',
+  version='2.7.0',
 
   author='Shuzhao Li, Francisco Castellanos, Andrei Todor',
   author_email='shuzhao.li@gmail.com',
   description='Pathway and network analysis for metabolomics data',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/shuzhao-li/mummichog',
@@ -38,14 +38,14 @@
   entry_points = {
         'console_scripts': ['mummichog=mummichog.command_line:main'],
     },
 
   python_requires='>=3.4',
   install_requires=[
     'matplotlib',
-    'networkx>=1,<2',
+    'networkx>=2',
     'numpy',
     'scipy',
     'xlsxwriter',
   ],
 
 )
```

