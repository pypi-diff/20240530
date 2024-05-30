# Comparing `tmp/yappgen-0.4.dev0.tar.gz` & `tmp/yappgen-0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappgen-0.4.dev0.tar", last modified: Thu May 23 16:25:53 2024, max compression
+gzip compressed data, was "yappgen-0.4.dev1.tar", last modified: Thu May 30 06:47:46 2024, max compression
```

## Comparing `yappgen-0.4.dev0.tar` & `yappgen-0.4.dev1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    26526 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/LICENSE
--rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/PKG-INFO
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      803 2024-04-24 07:23:10.000000 yappgen-0.4.dev0/README.md
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      781 2024-05-23 16:25:50.000000 yappgen-0.4.dev0/pyproject.toml
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      186 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/setup.cfg
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/yapp/
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      158 2024-05-23 16:13:53.000000 yappgen-0.4.dev0/src/yapp/__init__.py
--rwxrwxr-x   0 bservin   (1001) bservin   (1001)     5143 2024-05-23 16:07:40.000000 yappgen-0.4.dev0/src/yapp/cmd.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    36885 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/family_phaser.py
--rwxrwxr-x   0 bservin   (1001) bservin   (1001)     6130 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/fphtrain.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     8029 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/gamete.py
--rwxrwxr-x   0 bservin   (1001) bservin   (1001)    10173 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/lmm.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     5844 2024-04-24 07:25:07.000000 yappgen-0.4.dev0/src/yapp/mendel.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    17102 2024-05-23 16:05:13.000000 yappgen-0.4.dev0/src/yapp/origins.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    15828 2024-04-24 07:23:10.000000 yappgen-0.4.dev0/src/yapp/pedigree.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    20484 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/recombination.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     7179 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/sperm.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    11770 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/vcf.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     5873 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/wcsp.py
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/yappgen.egg-info/
--rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/PKG-INFO
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      510 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/SOURCES.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/dependency_links.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)       69 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/entry_points.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)       93 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/requires.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)        5 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/top_level.txt
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-30 06:47:46.820459 yappgen-0.4.dev1/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    26526 2023-04-12 12:19:27.000000 yappgen-0.4.dev1/LICENSE
+-rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-30 06:47:46.820459 yappgen-0.4.dev1/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      803 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/README.md
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      781 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/pyproject.toml
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      186 2024-05-30 06:47:46.824459 yappgen-0.4.dev1/setup.cfg
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-30 06:47:46.820459 yappgen-0.4.dev1/src/
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-30 06:47:46.820459 yappgen-0.4.dev1/src/yapp/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      159 2024-05-30 06:47:20.000000 yappgen-0.4.dev1/src/yapp/__init__.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     5143 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/cmd.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    36885 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/family_phaser.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     6130 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/fphtrain.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     8029 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/gamete.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)    10173 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/lmm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5844 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/mendel.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    17099 2024-05-30 06:46:24.000000 yappgen-0.4.dev1/src/yapp/origins.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    15828 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/pedigree.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    20484 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/recombination.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     7179 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/sperm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    11770 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/vcf.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5873 2024-05-30 06:45:30.000000 yappgen-0.4.dev1/src/yapp/wcsp.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-30 06:47:46.820459 yappgen-0.4.dev1/src/yappgen.egg-info/
+-rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      510 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       69 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/entry_points.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       93 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/requires.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        5 2024-05-30 06:47:46.000000 yappgen-0.4.dev1/src/yappgen.egg-info/top_level.txt
```

### Comparing `yappgen-0.4.dev0/LICENSE` & `yappgen-0.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/PKG-INFO` & `yappgen-0.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappgen
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Yet Another Phasing Program
 License: LGPL v2.1
 Project-URL: Repository, https://github.com/BertrandServin/yapp
 Project-URL: Documentation, https://yapp.readthedocs.io
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yappgen-0.4.dev0/README.md` & `yappgen-0.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/pyproject.toml` & `yappgen-0.4.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/cmd.py` & `yappgen-0.4.dev1/src/yapp/cmd.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/family_phaser.py` & `yappgen-0.4.dev1/src/yapp/family_phaser.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/fphtrain.py` & `yappgen-0.4.dev1/src/yapp/fphtrain.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/gamete.py` & `yappgen-0.4.dev1/src/yapp/gamete.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/lmm.py` & `yappgen-0.4.dev1/src/yapp/lmm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/mendel.py` & `yappgen-0.4.dev1/src/yapp/mendel.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/origins.py` & `yappgen-0.4.dev1/src/yapp/origins.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         logger.info("Tracing Ancestral Origins down the pedigree")
         smpidx = {}
         for i, name in enumerate(phaser.data["samples"]):
             smpidx[name] = i
         for reg in phaser.regions:
             logger.info(f"Working on region {reg}")
             segregations = np.array(phaser.data[f"phases/{reg}/segregations"])
-            origins = np.zeros_like(segregations, dtype=np.int)
+            origins = np.zeros_like(segregations, dtype=int)
             anc_origins = np.array(phaser.data[f"founders/{reg}/origins"])
             for node in phaser.pedigree:
                 node_idx = smpidx[node.indiv]
                 if node.father is None:
                     orig_0 = self.origins[node.indiv + "_p"]
                     origins[
                         node_idx,
```

### Comparing `yappgen-0.4.dev0/src/yapp/pedigree.py` & `yappgen-0.4.dev1/src/yapp/pedigree.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/recombination.py` & `yappgen-0.4.dev1/src/yapp/recombination.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/sperm.py` & `yappgen-0.4.dev1/src/yapp/sperm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/vcf.py` & `yappgen-0.4.dev1/src/yapp/vcf.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yapp/wcsp.py` & `yappgen-0.4.dev1/src/yapp/wcsp.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.4.dev0/src/yappgen.egg-info/PKG-INFO` & `yappgen-0.4.dev1/src/yappgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappgen
-Version: 0.4.dev0
+Version: 0.4.dev1
 Summary: Yet Another Phasing Program
 License: LGPL v2.1
 Project-URL: Repository, https://github.com/BertrandServin/yapp
 Project-URL: Documentation, https://yapp.readthedocs.io
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

