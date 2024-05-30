# Comparing `tmp/molecular_interaction_rules-0.1.tar.gz` & `tmp/molecular_interaction_rules-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.1.tar", last modified: Thu May 30 02:57:42 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.2.tar", last modified: Thu May 30 03:04:25 2024, max compression
```

## Comparing `molecular_interaction_rules-0.1.tar` & `molecular_interaction_rules-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:57:42.556145 molecular_interaction_rules-0.1/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.1/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 02:57:42.555681 molecular_interaction_rules-0.1/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)       42 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.1/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:57:42.550140 molecular_interaction_rules-0.1/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      130 2024-05-30 02:49:31.000000 molecular_interaction_rules-0.1/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6451 2024-05-30 02:49:30.000000 molecular_interaction_rules-0.1/molecular_interaction_rules/molecular_interaction_rules.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 02:57:42.554491 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 02:57:42.000000 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      400 2024-05-30 02:57:42.000000 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 02:57:42.000000 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 02:57:30.000000 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 02:57:42.000000 molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.1/requirements.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 02:57:42.556320 molecular_interaction_rules-0.1/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1657 2024-05-30 02:57:27.000000 molecular_interaction_rules-0.1/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:04:25.622059 molecular_interaction_rules-0.2/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.2/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 03:04:25.621568 molecular_interaction_rules-0.2/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       42 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.2/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:04:25.618955 molecular_interaction_rules-0.2/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      119 2024-05-30 03:03:55.000000 molecular_interaction_rules-0.2/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6464 2024-05-30 03:03:55.000000 molecular_interaction_rules-0.2/molecular_interaction_rules/knowledge_graph.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:04:25.620872 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 03:04:25.000000 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      388 2024-05-30 03:04:25.000000 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:04:25.000000 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:04:25.000000 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:04:25.000000 molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.2/requirements.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:04:25.622311 molecular_interaction_rules-0.2/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1657 2024-05-30 03:04:03.000000 molecular_interaction_rules-0.2/setup.py
```

### Comparing `molecular_interaction_rules-0.1/PKG-INFO` & `molecular_interaction_rules-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.1
+Version: 0.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Non-Covalent-Molecular-Interaction-Rules
 Keywords: molcules non-covalent interactions rules geometry
```

### Comparing `molecular_interaction_rules-0.1/molecular_interaction_rules/molecular_interaction_rules.py` & `molecular_interaction_rules-0.2/molecular_interaction_rules/knowledge_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 #
-# Lennard-Jones-Drill-2: Monomers
-# -------------------------------
+# Molecular Interation Rules: Knowledge Graph
+# -------------------------------------------
 
-class MolecularInteractionRules(object):
+class KnowledgeGraph(object):
 
     def __init__(self):
 
         self.master_list = []
 
         self.functional_group_mapping = {
           'aromatics': self.get_aromatics(),
```

### Comparing `molecular_interaction_rules-0.1/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.2/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.1
+Version: 0.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Non-Covalent-Molecular-Interaction-Rules
 Keywords: molcules non-covalent interactions rules geometry
```

### Comparing `molecular_interaction_rules-0.1/setup.py` & `molecular_interaction_rules-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.1",
+    version="0.2",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     install_requires=REQUIREMENTS,
     long_description=long_description,
```

