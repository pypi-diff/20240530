# Comparing `tmp/molecular_interaction_rules-0.5.6.tar.gz` & `tmp/molecular_interaction_rules-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_interaction_rules-0.5.6.tar", last modified: Thu May 30 03:42:29 2024, max compression
+gzip compressed data, was "molecular_interaction_rules-0.5.7.tar", last modified: Thu May 30 03:48:08 2024, max compression
```

## Comparing `molecular_interaction_rules-0.5.6.tar` & `molecular_interaction_rules-0.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:42:29.379315 molecular_interaction_rules-0.5.6/
--rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.6/MANIFEST.in
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:42:29.378672 molecular_interaction_rules-0.5.6/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.6/README.md
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:42:29.374112 molecular_interaction_rules-0.5.6/molecular_interaction_rules/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6921 2024-05-30 03:42:14.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules/molecular_database.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:42:29.377684 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:42:28.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:42:28.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:42:28.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:42:28.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:42:28.000000 molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:42:29.379488 molecular_interaction_rules-0.5.6/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:42:25.000000 molecular_interaction_rules-0.5.6/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.312028 molecular_interaction_rules-0.5.7/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       51 2024-05-29 19:10:30.000000 molecular_interaction_rules-0.5.7/MANIFEST.in
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:48:08.311610 molecular_interaction_rules-0.5.7/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      667 2024-05-30 03:16:25.000000 molecular_interaction_rules-0.5.7/README.md
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.308691 molecular_interaction_rules-0.5.7/molecular_interaction_rules/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      113 2024-05-30 03:30:03.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3134 2024-05-30 03:47:59.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules/molecular_database.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2024-05-30 03:48:08.310897 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2085 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      374 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       28 2024-05-30 03:48:07.000000 molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2024-05-30 03:48:08.312245 molecular_interaction_rules-0.5.7/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1698 2024-05-30 03:48:05.000000 molecular_interaction_rules-0.5.7/setup.py
```

### Comparing `molecular_interaction_rules-0.5.6/PKG-INFO` & `molecular_interaction_rules-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_interaction_rules
-Version: 0.5.6
+Version: 0.5.7
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.6/README.md` & `molecular_interaction_rules-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `molecular_interaction_rules-0.5.6/molecular_interaction_rules.egg-info/PKG-INFO` & `molecular_interaction_rules-0.5.7/molecular_interaction_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-interaction-rules
-Version: 0.5.6
+Version: 0.5.7
 Summary: UNKNOWN
 Home-page: https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: GPL
 Description: # Molecular Interaction Rules
```

### Comparing `molecular_interaction_rules-0.5.6/setup.py` & `molecular_interaction_rules-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     long_description = 'Non-Covalent Molecular Interaction Rules'
 
 # exec
 # ----
 setup(
     name="molecular_interaction_rules",
-    version="0.5.6",
+    version="0.5.7",
     packages=['molecular_interaction_rules'],
     license='GPL',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/mackerell-lab/Non-Covalent-Molecular-Interaction-Rules",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

