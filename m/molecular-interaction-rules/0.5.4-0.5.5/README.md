# Comparing `tmp/molecular_interaction_rules-0.5.4.tar.gz` & `tmp/molecular_interaction_rules-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.4.tar", last modified: Thu May 30 03:37:35 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.5.tar", last modified: Thu May 30 03:40:04 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.4.tar` & `molecular_interaction_rules-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:37:35.764344 molecular_interaction_rules-0.5.4/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.4/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:37:35.763208 molecular_interaction_rules-0.5.4/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.4/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:37:35.756555 molecular_interaction_rules-0.5.4/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6895 2024-05-30 03:31:51.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:37:35.762243 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:37:35.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:37:35.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:37:35.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:37:35.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:37:35.000000 molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:37:35.765424 molecular_interaction_rules-0.5.4/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:37:29.000000 molecular_interaction_rules-0.5.4/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:40:04.423159 molecular_interaction_rules-0.5.5/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.5/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:40:04.422621 molecular_interaction_rules-0.5.5/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.5/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:40:04.418923 molecular_interaction_rules-0.5.5/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6895 2024-05-30 03:31:51.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:40:04.421993 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:40:04.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:40:04.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:40:04.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:40:04.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:40:04.000000 molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:40:04.423359 molecular_interaction_rules-0.5.5/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:40:02.000000 molecular_interaction_rules-0.5.5/setup.py
```

### Comparing `molecular_interaction_rules-0.5.4/PKG-INFO` & `molecular_interaction_rules-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.4
+Version: 0.5.5
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.4/README.md` & `molecular_interaction_rules-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.4/molecular_interaction_rules/molecular_database.py` & `molecular_interaction_rules-0.5.5/molecular_interaction_rules/molecular_database.py`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.4/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.5/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.4
+Version: 0.5.5
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.4/setup.py` & `molecular_interaction_rules-0.5.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.4",
+    version="0.5.5",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

