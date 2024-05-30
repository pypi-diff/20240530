# Comparing `tmp/molecular_interaction_rules-0.5.7.tar.gz` & `tmp/molecular_interaction_rules-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.7.tar", last modified: Thu May 30 03:48:08 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.8.tar", last modified: Thu May 30 03:54:12 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.7.tar` & `molecular_interaction_rules-0.5.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.312028 molecular_interaction_rules-0.5.7/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.7/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:48:08.311610 molecular_interaction_rules-0.5.7/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.7/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.308691 molecular_interaction_rules-0.5.7/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3134 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.310897 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:48:08.312245 molecular_interaction_rules-0.5.7/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:48:05.000000 molecular_interaction_rules-0.5.7/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.706776 molecular_interaction_rules-0.5.8/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.8/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 03:54:12.706361 molecular_interaction_rules-0.5.8/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.8/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.701525 molecular_interaction_rules-0.5.8/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      224 2024-05-30 03:52:14.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3055 2024-05-30 03:50:44.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.705591 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:54:12.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:54:12.706918 molecular_interaction_rules-0.5.8/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:54:09.000000 molecular_interaction_rules-0.5.8/setup.py
```

### Comparing `molecular_interaction_rules-0.5.7/PKG-INFO` & `molecular_interaction_rules-0.5.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.7
+Version: 0.5.8
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
         
@@ -36,14 +36,21 @@
         
         #### Get Dimer Coordinates 
         
         ```python
         
         ```
         
+        Contact
+        =======
+        
+        Lead Developer: Suliman Sharif
+        Co-Authors: Anmol Kumar, Alexander D. MacKerell Jr.
+        
+        © Copyright 2024 – University of Maryland School of Pharmacy, Computer-Aided Drug Design Center All Rights Reserved
         
         
 Keywords: molcules non-covalent interactions rules geometry
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `molecular_interaction_rules-0.5.7/molecular_interaction_rules/molecular_database.py` & `molecular_interaction_rules-0.5.8/molecular_interaction_rules/molecular_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 #!/usr/bin/env python3
 #
 # Molecular Interation Rules: MoleculerDatabase
 # ---------------------------------------------
 
-from .molecules.aromatic.benzene import Benzene
+from molecular_interaction_rules.molecules.aromatic.benzene import Benzene
 
 class MoleculerDatabase(object):
 
     def __init__(self):
-        
+
         self.master_list = self.build_molecular_database()
-    
+
     def build_molecular_database(self):
-        
+
         molecules = [
-            
-            # Aromatics 
-          
+
+            # Aromatics
+
             Benzene()
         ]
-      
+
         return molecules
 
     def get_atom_names(self, monomer):
-        
-        ''' 
-        
+
+        '''
+
         Retrieve Atom Names of Molecule
-        
+
         '''
-        
+
         atom_names = []
 
         for molecule in self.get_master_list():
-  
+
             name = str(molecule.__name__).lower()
-    
+
             if name == monomer:
                 molecule = molecule()
                 atom_names = list(molecule.get_monomer_a_species().keys())
-        
+
         return atom_names
-          
+
     def get_monomer_coordinates(
       self,
       monomer,
       atom_name,
       monomer_b=False,
       functional_group_family=False
     ):
```

### Comparing `molecular_interaction_rules-0.5.7/setup.py` & `molecular_interaction_rules-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.7",
+    version="0.5.8",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

