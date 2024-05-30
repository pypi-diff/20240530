# Comparing `tmp/molecular_interaction_rules-0.3.tar.gz` & `tmp/molecular_interaction_rules-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.3.tar", last modified: Thu May 30 03:06:45 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.4.tar", last modified: Thu May 30 03:19:32 2024, max compression
```

## Comparing `molecular_interaction_rules-0.3.tar` & `molecular_interaction_rules-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:06:45.301339 molecular_interaction_rules-0.3/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.3/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 03:06:45.301041 molecular_interaction_rules-0.3/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)       42 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.3/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:06:45.294848 molecular_interaction_rules-0.3/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      107 2024-05-30 03:06:41.000000 molecular_interaction_rules-0.3/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6464 2024-05-30 03:03:55.000000 molecular_interaction_rules-0.3/molecular_interaction_rules/knowledge_graph.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:06:45.300552 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      925 2024-05-30 03:06:44.000000 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      388 2024-05-30 03:06:44.000000 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:06:44.000000 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:06:44.000000 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:06:44.000000 molecular_interaction_rules-0.3/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.3/requirements.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:06:45.301529 molecular_interaction_rules-0.3/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1657 2024-05-30 03:06:41.000000 molecular_interaction_rules-0.3/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:19:32.869263 molecular_interaction_rules-0.4/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.4/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1830 2024-05-30 03:19:32.868917 molecular_interaction_rules-0.4/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.4/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:19:32.865988 molecular_interaction_rules-0.4/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       96 2024-05-30 03:19:22.000000 molecular_interaction_rules-0.4/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6436 2024-05-30 03:19:22.000000 molecular_interaction_rules-0.4/molecular_interaction_rules/molecules.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:19:32.868291 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1830 2024-05-30 03:19:32.000000 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      382 2024-05-30 03:19:32.000000 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:19:32.000000 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:19:32.000000 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:19:32.000000 molecular_interaction_rules-0.4/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.4/requirements.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:19:32.869801 molecular_interaction_rules-0.4/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1657 2024-05-30 03:19:27.000000 molecular_interaction_rules-0.4/setup.py
```

### Comparing `molecular_interaction_rules-0.3/molecular_interaction_rules/knowledge_graph.py` & `molecular_interaction_rules-0.4/molecular_interaction_rules/molecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 #
-# Molecular Interation Rules: Knowledge Graph
-# -------------------------------------------
+# Molecular Interation Rules: Molecules
+# -------------------------------------
 
-class KnowledgeGraph(object):
+class Molecules(object):
 
     def __init__(self):
 
         self.master_list = []
 
         self.functional_group_mapping = {
           'aromatics': self.get_aromatics(),
@@ -168,15 +168,15 @@
         '''
 
         ions = self.get_ions()
 
         return ions[key]
 
 
-    def get_monomer_coordinates(
+    def get_monomer(
       self,
       monomer,
       atom_name,
       monomer_b=False,
       functional_group_family=False
     ):
 
@@ -210,15 +210,15 @@
 
             except KeyError as e:
                 print ('Missing Entry: %s | %s' % (name, atom_name))
                 return coordinates
 
             return coordinates, molecule.resi_name, rank_order
 
-    def get_dimer_coordinates(
+    def form_dimer_coordinates(
       self,
       molecule_name_1,
       atom_name_1,
       molecule_name_2,
       atom_name_2,
     ):
```

### Comparing `molecular_interaction_rules-0.3/setup.py` & `molecular_interaction_rules-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.3",
+    version="0.4",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     install_requires=REQUIREMENTS,
     long_description=long_description,
```

