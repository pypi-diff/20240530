# Comparing `tmp/molecular_interaction_rules-0.5.8.tar.gz` & `tmp/molecular_interaction_rules-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.8.tar", last modified: Thu May 30 03:54:12 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.9.tar", last modified: Thu May 30 04:00:53 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.8.tar` & `molecular_interaction_rules-0.5.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.706776 molecular_interaction_rules-0.5.8/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.8/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 03:54:12.706361 molecular_interaction_rules-0.5.8/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.8/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.701525 molecular_interaction_rules-0.5.8/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      224 2024-05-30 03:52:14.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3055 2024-05-30 03:50:44.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:54:12.705591 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:54:12.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:54:11.000000 molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:54:12.706918 molecular_interaction_rules-0.5.8/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:54:09.000000 molecular_interaction_rules-0.5.8/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:00:53.353354 molecular_interaction_rules-0.5.9/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.9/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 04:00:53.352982 molecular_interaction_rules-0.5.9/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      887 2024-05-30 03:52:35.000000 molecular_interaction_rules-0.5.9/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:00:53.349521 molecular_interaction_rules-0.5.9/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      122 2024-05-30 04:00:36.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3230 2024-05-30 03:59:52.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 04:00:53.352334 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2361 2024-05-30 04:00:53.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 04:00:53.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:00:53.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 04:00:53.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 04:00:53.000000 molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 04:00:53.353581 molecular_interaction_rules-0.5.9/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 04:00:40.000000 molecular_interaction_rules-0.5.9/setup.py
```

### Comparing `molecular_interaction_rules-0.5.8/PKG-INFO` & `molecular_interaction_rules-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.8/README.md` & `molecular_interaction_rules-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.8/molecular_interaction_rules/molecular_database.py` & `molecular_interaction_rules-0.5.9/molecular_interaction_rules/molecular_database.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 #!/usr/bin/env python3
 #
 # Molecular Interation Rules: MoleculerDatabase
 # ---------------------------------------------
 
-from molecular_interaction_rules.molecules.aromatic.benzene import Benzene
+# Imports
+# -------
+
+import os, sys
+
+# Reconfigurations
+# ----------------
+
+if os.name == 'nt':
+   sys.stdin.reconfigure(encoding='utf-8')
+   sys.stdout.reconfigure(encoding='utf-8')
+
+# Molecule Nodes
+
+from .molecules.aromatic.benzene import Benzene
 
 class MoleculerDatabase(object):
 
     def __init__(self):
 
         self.master_list = self.build_molecular_database()
```

### Comparing `molecular_interaction_rules-0.5.8/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.9/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.8/setup.py` & `molecular_interaction_rules-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.8",
+    version="0.5.9",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

