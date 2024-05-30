# Comparing `tmp/KIF-0.3.4.tar.gz` & `tmp/kif-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KIF-0.3.4.tar", last modified: Tue Feb 13 13:42:54 2024, max compression
+gzip compressed data, was "kif-0.4.0.tar", last modified: Thu May 30 14:54:22 2024, max compression
```

## Comparing `KIF-0.3.4.tar` & `kif-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 roryc760  (1000) roryc760  (1000)        0 2024-02-13 13:42:53.998577 KIF-0.3.4/
-drwxr-xr-x   0 roryc760  (1000) roryc760  (1000)        0 2024-02-13 13:42:53.988577 KIF-0.3.4/KIF.egg-info/
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)      643 2024-02-13 13:42:53.000000 KIF-0.3.4/KIF.egg-info/PKG-INFO
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)      894 2024-02-13 13:42:53.000000 KIF-0.3.4/KIF.egg-info/SOURCES.txt
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)        1 2024-02-13 13:42:53.000000 KIF-0.3.4/KIF.egg-info/dependency_links.txt
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)       82 2024-02-13 13:42:53.000000 KIF-0.3.4/KIF.egg-info/requires.txt
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)       24 2024-02-13 13:42:53.000000 KIF-0.3.4/KIF.egg-info/top_level.txt
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    18092 2023-10-03 12:54:20.000000 KIF-0.3.4/LICENSE.md
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)      643 2024-02-13 13:42:53.998577 KIF-0.3.4/PKG-INFO
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    10817 2023-10-03 12:54:20.000000 KIF-0.3.4/README.md
-drwxr-xr-x   0 roryc760  (1000) roryc760  (1000)        0 2024-02-13 13:42:53.998577 KIF-0.3.4/key_interactions_finder/
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)        0 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/__init__.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    11913 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/contact_identification.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    15032 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/data_preperation.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    35043 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/model_building.py
-drwxr-xr-x   0 roryc760  (1000) roryc760  (1000)        0 2024-02-13 13:42:53.998577 KIF-0.3.4/key_interactions_finder/model_params/
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)      409 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/model_params/gridsearch_custom.json
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)     4278 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/model_params/gridsearch_exhaustive.json
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)     2880 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/model_params/gridsearch_moderate.json
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)     1106 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/model_params/gridsearch_none.json
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)     1406 2023-10-03 12:54:20.000000 KIF-0.3.4/key_interactions_finder/model_params/gridsearch_quick.json
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    14144 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/network_analysis.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    35826 2024-02-13 10:27:26.000000 KIF-0.3.4/key_interactions_finder/post_proccessing.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    16771 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/pycontact_processing.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    11020 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/pymol_projections.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)    18834 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/stat_modelling.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)     7578 2024-02-13 10:04:58.000000 KIF-0.3.4/key_interactions_finder/utils.py
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)       38 2024-02-13 13:42:53.998577 KIF-0.3.4/setup.cfg
--rw-r--r--   0 roryc760  (1000) roryc760  (1000)      945 2024-02-13 13:42:48.000000 KIF-0.3.4/setup.py
+drwxrwxr-x   0 roryc     (1000) roryc     (1000)        0 2024-05-30 14:54:22.490140 kif-0.4.0/
+drwxrwxr-x   0 roryc     (1000) roryc     (1000)        0 2024-05-30 14:54:22.490140 kif-0.4.0/KIF.egg-info/
+-rw-r--r--   0 roryc     (1000) roryc     (1000)      643 2024-05-30 14:54:22.000000 kif-0.4.0/KIF.egg-info/PKG-INFO
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)      993 2024-05-30 14:54:22.000000 kif-0.4.0/KIF.egg-info/SOURCES.txt
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)        1 2024-05-30 14:54:22.000000 kif-0.4.0/KIF.egg-info/dependency_links.txt
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)       82 2024-05-30 14:54:22.000000 kif-0.4.0/KIF.egg-info/requires.txt
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)       24 2024-05-30 14:54:22.000000 kif-0.4.0/KIF.egg-info/top_level.txt
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    18092 2024-05-25 09:40:33.000000 kif-0.4.0/LICENSE.md
+-rw-r--r--   0 roryc     (1000) roryc     (1000)      643 2024-05-30 14:54:22.490140 kif-0.4.0/PKG-INFO
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    11084 2024-05-30 14:46:57.000000 kif-0.4.0/README.md
+drwxrwxr-x   0 roryc     (1000) roryc     (1000)        0 2024-05-30 14:54:22.490140 kif-0.4.0/key_interactions_finder/
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)        0 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/__init__.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     9670 2024-05-30 14:40:08.000000 kif-0.4.0/key_interactions_finder/chimerax_projections.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    11913 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/contact_identification.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    15032 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/data_preperation.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    35043 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_building.py
+drwxrwxr-x   0 roryc     (1000) roryc     (1000)        0 2024-05-30 14:54:22.490140 kif-0.4.0/key_interactions_finder/model_params/
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)      409 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_params/gridsearch_custom.json
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     4278 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_params/gridsearch_exhaustive.json
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     2880 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_params/gridsearch_moderate.json
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     1106 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_params/gridsearch_none.json
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     1406 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/model_params/gridsearch_quick.json
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    14144 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/network_analysis.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    35826 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/post_proccessing.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     2529 2024-05-30 14:40:08.000000 kif-0.4.0/key_interactions_finder/project_structure_utils.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    16771 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/pycontact_processing.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     9040 2024-05-30 14:40:08.000000 kif-0.4.0/key_interactions_finder/pymol_projections.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)    18834 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/stat_modelling.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)     7578 2024-05-25 09:40:33.000000 kif-0.4.0/key_interactions_finder/utils.py
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)       38 2024-05-30 14:54:22.490140 kif-0.4.0/setup.cfg
+-rw-rw-r--   0 roryc     (1000) roryc     (1000)      945 2024-05-30 14:42:29.000000 kif-0.4.0/setup.py
```

### Comparing `KIF-0.3.4/KIF.egg-info/PKG-INFO` & `kif-0.4.0/KIF.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KIF
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python package for MD simulation analysis
 Home-page: https://github.com/kamerlinlab/KIF
 Author: Rory Crean
 Author-email: rory.crean@kemi.uu.se
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.md
```

### Comparing `KIF-0.3.4/KIF.egg-info/SOURCES.txt` & `kif-0.4.0/KIF.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 setup.py
 KIF.egg-info/PKG-INFO
 KIF.egg-info/SOURCES.txt
 KIF.egg-info/dependency_links.txt
 KIF.egg-info/requires.txt
 KIF.egg-info/top_level.txt
 key_interactions_finder/__init__.py
+key_interactions_finder/chimerax_projections.py
 key_interactions_finder/contact_identification.py
 key_interactions_finder/data_preperation.py
 key_interactions_finder/model_building.py
 key_interactions_finder/network_analysis.py
 key_interactions_finder/post_proccessing.py
+key_interactions_finder/project_structure_utils.py
 key_interactions_finder/pycontact_processing.py
 key_interactions_finder/pymol_projections.py
 key_interactions_finder/stat_modelling.py
 key_interactions_finder/utils.py
 key_interactions_finder/model_params/gridsearch_custom.json
 key_interactions_finder/model_params/gridsearch_exhaustive.json
 key_interactions_finder/model_params/gridsearch_moderate.json
```

### Comparing `KIF-0.3.4/LICENSE.md` & `kif-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/PKG-INFO` & `kif-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KIF
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python package for MD simulation analysis
 Home-page: https://github.com/kamerlinlab/KIF
 Author: Rory Crean
 Author-email: rory.crean@kemi.uu.se
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.md
```

### Comparing `KIF-0.3.4/README.md` & `kif-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # KIF - Key Interactions Finder
  A python package to identify the key molecular interactions that regulate any conformational change.
 
- ### New in Version 0.3.0  - (14/07/2023)
+### New in Version 0.4.0 - (30/05/2024)
+
+Now KIF results can be projected onto a given 3D structure using [ChimeraX](https://www.cgl.ucsf.edu/chimerax/). Previously only [PyMOL](https://pymol.org/) was possible. Thanks to @darianyang for adding this functionality. 
+
+
+### New in Version 0.3.0  - (14/07/2023)
 The non-covalent interaction detection part of KIF has been rewritten to be much faster. 
 These changes have the biggest effect on larger systems.
 
 #### Example improvements:
 **Small trajectory of 214 residues and 98 frames.**
 - Old code: 5 min 54 seconds
 - New code: 29 seconds
```

### Comparing `KIF-0.3.4/key_interactions_finder/contact_identification.py` & `kif-0.4.0/key_interactions_finder/contact_identification.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/data_preperation.py` & `kif-0.4.0/key_interactions_finder/data_preperation.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/model_building.py` & `kif-0.4.0/key_interactions_finder/model_building.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/model_params/gridsearch_exhaustive.json` & `kif-0.4.0/key_interactions_finder/model_params/gridsearch_exhaustive.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/model_params/gridsearch_moderate.json` & `kif-0.4.0/key_interactions_finder/model_params/gridsearch_moderate.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/model_params/gridsearch_none.json` & `kif-0.4.0/key_interactions_finder/model_params/gridsearch_none.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/model_params/gridsearch_quick.json` & `kif-0.4.0/key_interactions_finder/model_params/gridsearch_quick.json`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/network_analysis.py` & `kif-0.4.0/key_interactions_finder/network_analysis.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/post_proccessing.py` & `kif-0.4.0/key_interactions_finder/post_proccessing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/pycontact_processing.py` & `kif-0.4.0/key_interactions_finder/pycontact_processing.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/pymol_projections.py` & `kif-0.4.0/key_interactions_finder/pymol_projections.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,23 @@
     Write out a PyMOL compatible python script to project the top features.
 
 4. project_multiple_per_feature_scores(all_feature_scores, numb_features, out_dir)
     Write out multiple PyMOL compatible scripts for different models.
 
 """
 from pathlib import Path
-from typing import Union, Tuple
+from typing import Union
 import pandas as pd
 from key_interactions_finder.utils import _prep_out_dir
+from key_interactions_finder.project_structure_utils import (
+    _extract_residue_lists, 
+    _write_file, 
+    _extract_interaction_types, 
+    _scale_interaction_strengths
+)
 
 
 def project_pymol_per_res_scores(per_res_scores: dict,
                                  model_name: str = "",
                                  out_dir: str = ""
                                  ) -> None:
     """
@@ -212,86 +218,7 @@
         project_pymol_top_features(
             per_feature_scores=model_scores,
             model_name=model_name,
             numb_features=numb_features,
             out_dir=out_dir
         )
 
-
-def _extract_residue_lists(input_df: pd.DataFrame) -> Tuple[list, list]:
-    """
-    Extract two list of residues that are present in each feature.
-
-    Parameters
-    ----------
-
-    input_df : pd.DataFrame
-        Dataframe of feature names.
-
-    Returns
-    ----------
-    
-    res1 : list
-        residue 1 for each feature.
-
-    res2 : list
-        residue 2 for each feature.
-    """
-    residue1 = (input_df[0].str.extract(
-        r"(\d+)")).astype(int).values.tolist()
-    residue2 = (input_df[1].str.extract(
-        r"(\d+)")).astype(int).values.tolist()
-    res1 = [item for sublist in residue1 for item in sublist]
-    res2 = [item for sublist in residue2 for item in sublist]
-
-    return res1, res2
-
-
-def _write_file(file_name: str, text: str) -> None:
-    """Write out a PyMOL text file."""
-    with open(file_name, "w+", encoding="utf-8") as file_out:
-        file_out.write(text)
-
-
-def _extract_interaction_types(input_df: pd.DataFrame) -> list:
-    """
-    Extract the interaction type for each feature and what colour scheme to use.
-
-    Parameters
-    ----------
-    input_df : pd.DataFrame
-        Dataframe of feature names.
-
-    Returns
-    ----------
-    list
-        List of colors to assign for each feature.
-    """
-    stick_col_scheme = {"Hbond": "red", "Saltbr": "blue",
-                        "Hydrophobic": "green", "Other": "magenta"}
-
-    interact_type = input_df[2].values.tolist()
-    return [stick_col_scheme[i] for i in interact_type if i in stick_col_scheme]
-
-
-def _scale_interaction_strengths(input_df: pd.DataFrame) -> list:
-    """
-    Determine interaction strength value and scale so max is 0.5 (Good for PyMOL).
-
-    Parameters
-    ----------
-    input_df : pd.DataFrame
-        Dataframe of per feature scores.
-
-    Returns
-    ----------
-    list
-        Scaled and rounded per feature scores.
-    """
-    interact_strengths = input_df[1]
-    max_strength = max(interact_strengths)
-
-    interact_strengths_scaled = []
-    for interaction in interact_strengths:
-        interact_strengths_scaled.append(interaction / max_strength / 2)
-
-    return [round(elem, 4) for elem in interact_strengths_scaled]
```

### Comparing `KIF-0.3.4/key_interactions_finder/stat_modelling.py` & `kif-0.4.0/key_interactions_finder/stat_modelling.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/key_interactions_finder/utils.py` & `kif-0.4.0/key_interactions_finder/utils.py`

 * *Files identical despite different names*

### Comparing `KIF-0.3.4/setup.py` & `kif-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.3.4"
+VERSION = "0.4.0"
 DESCRIPTION = "Python package for MD simulation analysis"
 LONG_DESCRIPTION = """
     A python package to identify the key molecular interactions that regulate any conformational change."""
 
 setup(
     name="KIF",
     version=VERSION,
```

