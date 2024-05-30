# Comparing `tmp/onion_clustering-0.2.5.tar.gz` & `tmp/onion_clustering-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.2.5.tar", last modified: Mon May 20 13:18:12 2024, max compression
+gzip compressed data, was "onion_clustering-0.2.6.tar", last modified: Tue May 21 08:17:04 2024, max compression
```

## Comparing `onion_clustering-0.2.5.tar` & `onion_clustering-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.018379 onion_clustering-0.2.5/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-20 12:56:22.000000 onion_clustering-0.2.5/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.5/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-20 13:18:12.017837 onion_clustering-0.2.5/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5465 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.000934 onion_clustering-0.2.5/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3647 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3637 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-20 13:17:00.000000 onion_clustering-0.2.5/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.5/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-20 13:18:12.018501 onion_clustering-0.2.5/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:11.994341 onion_clustering-0.2.5/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.007919 onion_clustering-0.2.5/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    30001 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    26453 2024-05-20 12:51:45.000000 onion_clustering-0.2.5/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-17 12:50:03.000000 onion_clustering-0.2.5/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.017125 onion_clustering-0.2.5/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-20 13:18:11.000000 onion_clustering-0.2.5/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.012047 onion_clustering-0.2.5/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.5/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.014143 onion_clustering-0.2.5/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-20 13:18:12.016286 onion_clustering-0.2.5/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1662 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     2941 2024-05-20 09:25:02.000000 onion_clustering-0.2.5/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.186690 onion_clustering-0.2.6/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-05-21 08:12:51.000000 onion_clustering-0.2.6/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       81 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.2.6/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-21 08:17:04.185618 onion_clustering-0.2.6/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5465 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.164949 onion_clustering-0.2.6/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3647 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3637 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      641 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      947 2024-05-21 08:05:43.000000 onion_clustering-0.2.6/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.2.6/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-05-21 08:17:04.187104 onion_clustering-0.2.6/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.155701 onion_clustering-0.2.6/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.169993 onion_clustering-0.2.6/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    36398 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20386 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    30001 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    26152 2024-05-21 08:06:28.000000 onion_clustering-0.2.6/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    20729 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-05-17 12:50:03.000000 onion_clustering-0.2.6/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.184359 onion_clustering-0.2.6/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5901 2024-05-21 08:17:04.000000 onion_clustering-0.2.6/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      842 2024-05-21 08:17:04.000000 onion_clustering-0.2.6/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-05-21 08:17:04.000000 onion_clustering-0.2.6/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-05-21 08:17:04.000000 onion_clustering-0.2.6/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-05-21 08:17:04.000000 onion_clustering-0.2.6/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.176685 onion_clustering-0.2.6/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.2.6/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.180110 onion_clustering-0.2.6/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      412 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-05-21 08:17:04.183434 onion_clustering-0.2.6/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1746 2024-05-21 08:05:43.000000 onion_clustering-0.2.6/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-05-21 08:05:43.000000 onion_clustering-0.2.6/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-05-21 08:05:43.000000 onion_clustering-0.2.6/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3112 2024-05-20 09:25:02.000000 onion_clustering-0.2.6/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     2916 2024-05-21 08:05:43.000000 onion_clustering-0.2.6/test/test_uni.py
```

### Comparing `onion_clustering-0.2.5/.coverage` & `onion_clustering-0.2.6/.coverage`

 * *Files 5% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -48,16 +48,16 @@
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
 INSERT INTO line_bits VALUES(2,1,X'c27b0790e0e60750fe010000008edec94b7e07f91d2c37843fbfaffffdde000000000000000000000000f90300d27df3c97b1cf201c8f9fc85b53d7d7e000000762b789a0700a09180edf97fbfcf7900ef12');
 INSERT INTO line_bits VALUES(3,1,X'627f819075ff4564c9f37bbb029de2342ac68fdfe493593e052c220000000000840b00000090bbe7e7dd2768db75af3b56fc3e3ff271cb0479bf7f92f7f9317e5efee7e779f7fbfdf8962625db3f6e5680db5d7f7efcfffdfd3100008005b020efdfffc45f00000000000000000000000080f9bd7ffff3efbf7ffff1972db3fcec3f6e');
 INSERT INTO line_bits VALUES(4,1,X'625f0200c0f85dc08c5f40c66308c00b0858000080c0b74040003bc636f3fd1e3ffff7e79f2fe36100c66701020bfc9e00404084c7d866dee3e77fff7c190ffcbfefefbb11c02bfeff0b');
-INSERT INTO line_bits VALUES(5,1,X'a25f0230280f008003780000b4af96070080070080f6ad1c0000f01800e8f6db776500c0aed75bf90700000000cfddbf1c00200f0000481e8b250000007fc37940010000ee5e9b5b1e0000766ffe7ff2010000bcbf179e87ff00c7fbe6e7930f000000fff907000000fcbddddbc9010088470eff93ff16cf3fbff171be5b');
-INSERT INTO line_bits VALUES(6,1,X'c2f70ec00400c019f203281f00000000e0edff97ff8dfc010000c07c3ecccfe3e7f1ff6efbfd0a00407e00000090bb9b4fdee3917f00000090cb87f5cbe3e77107d3df7cc97b1c820f000000ce3ebf33fe73df3d3f000000bb153c7f9ee60100d078fee400607bfeb7dfe73c000000807709');
+INSERT INTO line_bits VALUES(5,1,X'a25f0230280f008003780000b4af96070080070080f6ad1c0000f01800e8f6db776500c0aed75bf90700000000cfddbf1c00200f0000481e8b250000007fc37940010000ee5e9b5b1e0000766ffe7ff2010000bcbf7f9e83ff16c7fbe6e7930f000000fff907000000fcbddddbc9010088470eff93ff16cf3fbff171be5b');
+INSERT INTO line_bits VALUES(6,1,X'c2f71d8009008033e407503e00000000c0dbff2fff1ef90300008039e7e7f1f3f87887fd7e0500203f000000c8ddcd27eff1c83f000000c8e5c3fae1f1f3a883e96fbee43d0ec907000000679f5f18ffb9ef9e1f000080dd0a9e3f4ff30000683c7f7200b03dffdbef731e000000c0bb04');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `onion_clustering-0.2.5/LICENSE` & `onion_clustering-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/PKG-INFO` & `onion_clustering-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.5
+Version: 0.2.6
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.5/README.md` & `onion_clustering-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/examples/example_script.py` & `onion_clustering-0.2.6/examples/example_script.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/examples/example_script_2d.py` & `onion_clustering-0.2.6/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/justfile` & `onion_clustering-0.2.6/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/pyproject.toml` & `onion_clustering-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.2.5"
+version = "0.2.6"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.2.5/src/onion_clustering/classes.py` & `onion_clustering-0.2.6/src/onion_clustering/classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/src/onion_clustering/first_classes.py` & `onion_clustering-0.2.6/src/onion_clustering/first_classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/src/onion_clustering/functions.py` & `onion_clustering-0.2.6/src/onion_clustering/functions.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/src/onion_clustering/main.py` & `onion_clustering-0.2.6/src/onion_clustering/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import warnings
 from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal
 from scipy.optimize import OptimizeWarning
+from scipy.stats import gaussian_kde
 
 from onion_clustering.classes import ClusteringObject1D
 from onion_clustering.first_classes import Parameters, StateUni, UniData
 from onion_clustering.functions import (
     gaussian,
     max_prob_assignment,
     moving_average,
@@ -211,32 +212,22 @@
         Object containing Gaussian fit parameters (mu, sigma, area)
         or None if the fit fails.
     """
     print("* Gaussian fit...")
     flat_m = m_clean.flatten()
 
     ### 1. Histogram ###
-    counts, bins = np.histogram(flat_m, bins=par.bins, density=True)
-    gap = 1
-    if bins.size > 49:
-        gap = int(bins.size * 0.02) * 2
-    print(f"\tNumber of bins = {bins.size}, gap = {gap}")
-
-    ### 2. Smoothing with tau = 3 ###
-    counts = moving_average(counts, gap)
-    bins = moving_average(bins, gap)
-    if (counts == 0.0).any():
-        print(
-            "\tWARNING: there are empty bins. "
-            "Consider reducing the number of bins."
-        )
+    kde = gaussian_kde(flat_m)
+    bins = np.linspace(np.min(flat_m), np.max(flat_m), 1000)
+    counts = kde.evaluate(bins)
 
     ### 3. Find the maximum ###
     max_val = counts.max()
     max_ind = counts.argmax()
+    gap = 3
 
     ### 4. Find the minima surrounding it ###
     min_id0 = np.max([max_ind - gap, 0])
     min_id1 = np.min([max_ind + gap, counts.size - 1])
     while min_id0 > 0 and counts[min_id0] > counts[min_id0 - 1]:
         min_id0 -= 1
     while min_id1 < counts.size - 1 and counts[min_id1] > counts[min_id1 + 1]:
```

### Comparing `onion_clustering-0.2.5/src/onion_clustering/main_2d.py` & `onion_clustering-0.2.6/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/src/onion_clustering/utilities.py` & `onion_clustering-0.2.6/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.2.6/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.2.5
+Version: 0.2.6
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.2.5/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.2.6/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/test/test_multi.py` & `onion_clustering-0.2.6/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.2.5/test/test_uni.py` & `onion_clustering-0.2.6/test/test_uni.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 def test_output_files(setup_test_environment):
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
-        print("tau_window\t" + str(TAU_WINDOW), file=file)
-        print("t_delay\t" + str(T_DELAY), file=file)
-        print("num_tau_w\t" + str(NUM_TAU_W), file=file)
-        print("max_tau_w\t" + str(MAX_TAU_W), file=file)
-        print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
+        print(f"tau_window\t{TAU_WINDOW}", file=file)
+        print(f"t_delay\t{T_DELAY}", file=file)
+        print(f"num_tau_w\t{NUM_TAU_W}", file=file)
+        print(f"max_tau_w\t{MAX_TAU_W}", file=file)
+        print(f"max_t_smooth\t{MAX_T_SMOOTH}", file=file)
 
     # Call your code to generate the output files
     tmp = onion.main(False)
 
     # Test the output
     tmp.plot_tra_figure()
     tmp.plot_input_data("Fig0")
```

