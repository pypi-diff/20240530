# Comparing `tmp/molecular_interaction_rules-0.5.1.tar.gz` & `tmp/molecular_interaction_rules-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.1.tar", last modified: Thu May 30 03:26:54 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.2.tar", last modified: Thu May 30 03:30:17 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.1.tar` & `molecular_interaction_rules-0.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:26:54.578532 molecular_interaction_rules-0.5.1/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.1/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:26:54.577738 molecular_interaction_rules-0.5.1/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.1/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:26:54.572719 molecular_interaction_rules-0.5.1/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       96 2024-05-30 03:19:22.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6888 2024-05-30 03:26:09.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules/molecules.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:26:54.576760 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:26:54.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      365 2024-05-30 03:26:54.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:26:54.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:26:54.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:26:54.000000 molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:26:54.579403 molecular_interaction_rules-0.5.1/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:26:52.000000 molecular_interaction_rules-0.5.1/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:30:17.306679 molecular_interaction_rules-0.5.2/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.2/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:30:17.306245 molecular_interaction_rules-0.5.2/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.2/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:30:17.302364 molecular_interaction_rules-0.5.2/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6922 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:30:17.305570 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:30:16.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:30:16.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:30:16.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:30:16.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:30:16.000000 molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:30:17.306837 molecular_interaction_rules-0.5.2/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.2/setup.py
```

### Comparing `molecular_interaction_rules-0.5.1/PKG-INFO` & `molecular_interaction_rules-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.1
+Version: 0.5.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.1/README.md` & `molecular_interaction_rules-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.1/molecular_interaction_rules/molecules.py` & `molecular_interaction_rules-0.5.2/molecular_interaction_rules/molecular_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 #
-# Molecular Interation Rules: Molecules
-# -------------------------------------
+# Molecular Interation Rules: MoleculerDatabase
+# ---------------------------------------------
 
-class Molecules(object):
+class MoleculerDatabase(object):
 
     def __init__(self):
 
         self.master_list = []
 
         self.functional_group_mapping = {
           'aromatics': self.get_aromatics(),
@@ -30,15 +30,15 @@
 
         from molecular_interaction_rules.ions import __all__
 
         return __all__
 
     def get_aromatics(self):
 
-        from molecular_interaction_rules.aromatic import __all__
+        from molecular_interaction_rules.molecules.aromatic import __all__
 
         return __all__
 
     def get_alcohols(self):
 
         from molecular_interaction_rules.molecules.non_aromatic.alcohols import __all__
```

### Comparing `molecular_interaction_rules-0.5.1/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.2/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.1
+Version: 0.5.2
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.1/setup.py` & `molecular_interaction_rules-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.1",
+    version="0.5.2",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

