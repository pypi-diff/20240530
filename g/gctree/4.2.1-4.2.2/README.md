# Comparing `tmp/gctree-4.2.1.tar.gz` & `tmp/gctree-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gctree-4.2.1.tar", last modified: Fri Apr 12 02:58:59 2024, max compression
+gzip compressed data, was "gctree-4.2.2.tar", last modified: Thu May 30 18:00:56 2024, max compression
```

## Comparing `gctree-4.2.1.tar` & `gctree-4.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-12 02:58:50.000000 gctree-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 02:58:50.000000 gctree-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-12 02:58:59.064236 gctree-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 02:58:50.000000 gctree-4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86336 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/branching_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/isotyping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/mkconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/mutation_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/phylip_parse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-04-12 02:58:50.000000 gctree-4.2.1/gctree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/gctree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 02:58:59.000000 gctree-4.2.1/gctree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 02:58:59.064236 gctree-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 02:58:50.000000 gctree-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:58:59.064236 gctree-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_disambiguate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_isotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-12 02:58:50.000000 gctree-4.2.1/tests/test_local_branching.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 02:58:50.000000 gctree-4.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:00:56.917913 gctree-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-30 18:00:52.000000 gctree-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 18:00:52.000000 gctree-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-30 18:00:56.917913 gctree-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 18:00:52.000000 gctree-4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:00:56.913912 gctree-4.2.2/gctree/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 18:00:56.917913 gctree-4.2.2/gctree/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86334 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/branching_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26814 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7708 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/isotyping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2371 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/mkconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/mutation_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/phylip_parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1159 2024-05-30 18:00:52.000000 gctree-4.2.2/gctree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:00:56.917913 gctree-4.2.2/gctree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 18:00:56.000000 gctree-4.2.2/gctree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 18:00:56.917913 gctree-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-30 18:00:52.000000 gctree-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:00:56.917913 gctree-4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-30 18:00:52.000000 gctree-4.2.2/tests/test_disambiguate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-30 18:00:52.000000 gctree-4.2.2/tests/test_isotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-30 18:00:52.000000 gctree-4.2.2/tests/test_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-30 18:00:52.000000 gctree-4.2.2/tests/test_local_branching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-30 18:00:52.000000 gctree-4.2.2/versioneer.py
```

### Comparing `gctree-4.2.1/LICENSE` & `gctree-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/PKG-INFO` & `gctree-4.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.2.1
+Version: 4.2.2
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.2.1/README.md` & `gctree-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/branching_processes.py` & `gctree-4.2.2/gctree/branching_processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,15 @@
             vmax: maximum value for colormap (default to maximum of the feature over the tree)
             scale: ``linear`` (default), ``log``, or ``symlog`` (must also provide ``linthresh`` kwarg)
             kwargs: additional keyword arguments for scale transformation
 
         Returns:
             Dictionary of node names to hex color strings, which may be used as the colormap in :meth:`gctree.CollapsedTree.render`
         """
-        cmap = mp.cm.get_cmap(cmap)
+        cmap = mp.colormaps[cmap]
 
         if vmin is None:
             vmin = np.nanmin([getattr(node, feature) for node in self.tree.traverse()])
         if vmax is None:
             vmax = np.nanmax([getattr(node, feature) for node in self.tree.traverse()])
 
         if scale == "linear":
```

### Comparing `gctree-4.2.1/gctree/cli.py` & `gctree-4.2.2/gctree/cli.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/deduplicate.py` & `gctree-4.2.2/gctree/deduplicate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/isotype.py` & `gctree-4.2.2/gctree/isotype.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/isotyping.py` & `gctree-4.2.2/gctree/isotyping.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/mkconfig.py` & `gctree-4.2.2/gctree/mkconfig.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/mutation_model.py` & `gctree-4.2.2/gctree/mutation_model.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree/phylip_parse.py` & `gctree-4.2.2/gctree/phylip_parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,22 @@
 from ete3 import Tree
 import re
 import random
 from collections import defaultdict
 
 import pickle
 import argparse
+from warnings import warn
 from typing import Dict
 
+
+class TreeParseError(RuntimeError):
+    pass
+
+
 code_vectors = {
     code: [
         0 if base in gctree.utils.ambiguous_dna_values[code] else float("inf")
         for base in gctree.utils.bases
     ]
     for code in gctree.utils.ambiguous_dna_values
 }
@@ -91,52 +97,102 @@
                 last_blank = True
                 continue
         else:
             break
     return seqs
 
 
+def get_expected_trees(outfile):
+    with open(outfile) as fh:
+        for line, _ in zip(fh, range(7)):
+            if "trees in all found" in line:
+                return int(line.strip().split()[0])
+                break
+        else:
+            return None
+
+
 # parse the dnaml output file and return data structures containing a
 # list biopython.SeqRecords and a dict containing adjacency
 # relationships and distances between nodes.
 def parse_outfile(outfile, abundance_file=None, root="root", disambiguate=False):
     """Parse phylip outfile, and return dnapars trees."""
+    _expected_seq_len = None
+    _expected_n_trees = get_expected_trees(outfile)
+    _n_trees_warned = False
     if abundance_file is not None:
         counts = {
             line.split(",")[0]: int(line.split(",")[1]) for line in open(abundance_file)
         }
     # No count, just make an empty count dictionary:
     else:
         counts = None
     trees = []
     bootstrap = False
     # Ugg... for compilation need to let python know that these will definely both be defined :-/
     sequences, parents = {}, {}
     with open(outfile, "r") as fh:
         for sect in sections(fh):
-            if sect == "parents":
-                parents = {child: parent for child, parent in iter_edges(fh)}
-            elif sect[0] == "sequences":
-                sequences = parse_seqdict(fh, sect[1])
-                # sanity check;  a valid tree should have exactly one node that is parentless
-                if not len(parents) == len(sequences) - 1:
-                    raise RuntimeError(
-                        "invalid results attempting to parse {}: there are {} parentless sequences".format(
-                            outfile, len(sequences) - len(parents)
+            try:
+                if sect == "parents":
+                    parents = {child: parent for child, parent in iter_edges(fh)}
+                elif sect[0] == "sequences":
+                    sequences = parse_seqdict(fh, sect[1])
+                    # sanity check;  a valid tree should have exactly one node that is parentless
+                    if not len(parents) == len(sequences) - 1:
+                        raise TreeParseError(
+                            "invalid results attempting to parse {}: there are {} parentless sequences".format(
+                                outfile, len(sequences) - len(parents)
+                            )
+                        )
+                    # Also, all sequences should have the same length!
+                    _seq_lengths = list(set(len(seq) for _, seq in sequences.items()))
+                    if not len(_seq_lengths) == 1:
+                        raise TreeParseError(
+                            "Parsed node sequences do not all have the same length!"
                         )
+                    # Also, all sequences' lengths should match first tree's
+                    # seq lengths
+                    if _expected_seq_len is not None:
+                        if not _seq_lengths[0] == _expected_seq_len:
+                            raise TreeParseError(
+                                "Parsed tree node sequences don't match first parsed tree's sequences!"
+                            )
+                    else:
+                        _expected_seq_len = _seq_lengths[0]
+
+                    if bootstrap:
+                        trees[-1].append(build_tree(sequences, parents, counts, root))
+                    else:
+                        trees.append(build_tree(sequences, parents, counts, root))
+                elif sect == "seqboot_dataset":
+                    bootstrap = True
+                    trees.append([])
+                else:
+                    raise TreeParseError(
+                        "unrecognized phylip section = {}".format(sect)
                     )
-                if bootstrap:
-                    trees[-1].append(build_tree(sequences, parents, counts, root))
+            except TreeParseError:
+                if _expected_n_trees is not None:
+                    expected_message = f" but {_expected_n_trees} were expected"
                 else:
-                    trees.append(build_tree(sequences, parents, counts, root))
-            elif sect == "seqboot_dataset":
-                bootstrap = True
-                trees.append([])
-            else:
-                raise RuntimeError("unrecognized phylip section = {}".format(sect))
+                    expected_message = ""
+                warn(
+                    f"Error parsing {outfile}! {len(trees)} successfully read{expected_message}."
+                )
+                _n_trees_warned = True
+                break
+        if (
+            not _n_trees_warned
+            and _expected_n_trees is not None
+            and _expected_n_trees != len(trees)
+        ):
+            warn(
+                f"Parsed {len(trees)} from {outfile} but {_expected_n_trees} expected!"
+            )
     if len(trees) == 0:
         raise RuntimeError(f"No trees found in '{outfile}'")
     if disambiguate:
         # Disambiguate sets node.dist for all nodes in disambiguated trees
         trees = [disambiguate(tree) for tree in trees]
     return trees
```

### Comparing `gctree-4.2.1/gctree/utils.py` & `gctree-4.2.2/gctree/utils.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/gctree.egg-info/PKG-INFO` & `gctree-4.2.2/gctree.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gctree
-Version: 4.2.1
+Version: 4.2.2
 Summary: phylogenetic inference of genotype-collapsed trees
 Home-page: https://github.com/matsengrp/gctree
 Author: Matsen Group
 Author-email: ematsen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `gctree-4.2.1/gctree.egg-info/SOURCES.txt` & `gctree-4.2.2/gctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/setup.py` & `gctree-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/tests/test_disambiguate.py` & `gctree-4.2.2/tests/test_disambiguate.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/tests/test_isotype.py` & `gctree-4.2.2/tests/test_isotype.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/tests/test_likelihoods.py` & `gctree-4.2.2/tests/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/tests/test_local_branching.py` & `gctree-4.2.2/tests/test_local_branching.py`

 * *Files identical despite different names*

### Comparing `gctree-4.2.1/versioneer.py` & `gctree-4.2.2/versioneer.py`

 * *Files identical despite different names*

