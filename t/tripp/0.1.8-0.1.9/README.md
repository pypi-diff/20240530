# Comparing `tmp/tripp-0.1.8.tar.gz` & `tmp/tripp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripp-0.1.8.tar", max compression
+gzip compressed data, was "tripp-0.1.9.tar", max compression
```

## Comparing `tripp-0.1.8.tar` & `tripp-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-04-09 14:03:48.874947 tripp-0.1.8/LICENSE
--rw-r--r--   0        0        0     1397 2024-04-09 14:03:48.875120 tripp-0.1.8/README.md
--rw-r--r--   0        0        0      469 2024-04-12 09:50:41.826672 tripp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8118 2024-04-09 15:07:38.243777 tripp-0.1.8/tripp/Trajectory.py
--rw-r--r--   0        0        0     5231 2024-04-12 08:45:27.285532 tripp-0.1.8/tripp/Visualization.py
--rw-r--r--   0        0        0      210 2024-04-10 12:16:57.816361 tripp-0.1.8/tripp/__init__.py
--rw-r--r--   0        0        0    11753 2024-04-09 14:04:18.121635 tripp-0.1.8/tripp/color_palettes.py
--rw-r--r--   0        0        0     5454 2024-04-11 13:00:42.597583 tripp-0.1.8/tripp/edit_pdb.py
--rw-r--r--   0        0        0     1292 2024-04-09 14:04:18.121985 tripp-0.1.8/tripp/model_pka_values.py
--rw-r--r--   0        0        0     3019 2024-04-12 09:44:23.895197 tripp-0.1.8/tripp/visualise_pka.py
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 tripp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 14:03:48.874947 tripp-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1397 2024-04-09 14:03:48.875120 tripp-0.1.9/README.md
+-rw-r--r--   0        0        0      469 2024-04-12 10:50:24.735056 tripp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8118 2024-04-09 15:07:38.243777 tripp-0.1.9/tripp/Trajectory.py
+-rw-r--r--   0        0        0     6364 2024-04-12 10:40:52.368816 tripp-0.1.9/tripp/Visualization.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:16:57.816361 tripp-0.1.9/tripp/__init__.py
+-rw-r--r--   0        0        0     5454 2024-04-11 13:00:42.597583 tripp-0.1.9/tripp/edit_pdb.py
+-rw-r--r--   0        0        0     1292 2024-04-09 14:04:18.121985 tripp-0.1.9/tripp/model_pka_values.py
+-rw-r--r--   0        0        0     4223 2024-04-12 10:40:18.087942 tripp-0.1.9/tripp/visualize_pka.py
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 tripp-0.1.9/PKG-INFO
```

### Comparing `tripp-0.1.8/LICENSE` & `tripp-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tripp-0.1.8/README.md` & `tripp-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tripp-0.1.8/tripp/Trajectory.py` & `tripp-0.1.9/tripp/Trajectory.py`

 * *Files identical despite different names*

### Comparing `tripp-0.1.8/tripp/Visualization.py` & `tripp-0.1.9/tripp/Visualization.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,58 +20,72 @@
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 import MDAnalysis as mda
 import numpy as np
 import pandas as pd 
-from tripp.visualise_pka import visualise_pka 
+from tripp.visualize_pka import visualize_pka 
 from tripp.model_pka_values import model_pka_values 
 
 class Visualization: 
 
 
     """ 
-    This class allows for the visualisation of pKa values using PyMOL. The 
+    This class allows for the visualization of pKa values using PyMOL. The 
     class is called using a strucutre of the protein and a CSV file generated 
-    by the Trajectory class containing all pKa values. The method color_pka 
-    can be called which generated a PyMOL session file. The arguments of 
-    color_pka are the following: 
+    by the Trajectory class containing all pKa values.
     
-    coloring_method: 'mean' or 'difference_to_model_value' 
-    used to determine how the color of each residue is produced. Can be 'mean', 
-    where the mean pKa value accross all frames is used or 
-    'difference_to_model_value' where the mean pKa value is calculated 
-    and the difference to the model value of the amino acid in solution is 
-    used. 
-    
-    lower limit: int or float 
-    determines lower limit used to colour the reisdues in the PyMOL session. Any 
-    value below the limit is coloured using the lowest end of the color gradient 
-    used. 
-    
-    upper limit: int or float 
-    determines upper limit used to colour the reisdues in the PyMOL session. Any 
-    value above the limit is coloured using the highest end of the color gradient 
-    used. 
-
-    color_palette: 'red_white_blue', 'blue_white_red', 'red_white_green', and 'green_white_red' 
-    color palettes used to color the residues in the PyMOL session according to 
-    pKa value. The defaults is set to 'red_white_blue'. 
     """
 
 
     def __init__(self, structure, pka_file):
 
         self.structure = structure
         self.pka_file = pka_file
         
 
-    def color_pka(self, pymol_path, pse_output_prefix, coloring_method, lower_limit, upper_limit, color_palette='red_white_blue'): 
-        
+    def color_pka(self, pymol_path, pse_output_prefix, coloring_method='mean', lower_limit=0, upper_limit=14, color_palette='red_white_blue'): 
+        """
+        The method color_pka can be called which generate a PyMOL session file.
+        
+        Parameters:
+        
+        pymol_path: str
+        Path to the PyMOL software needs to be specified. The script will spawn
+        a subprocess shell to run a python script in PyMOL. Preventing packaging 
+        issue.
+        
+        pse_output_prefix: str
+        The output prefix for the PyMOL .pse file. The prefix will be combined 
+        with the coloring_method ('mean' or 'difference_to_model_value') to give
+        the pse_output_filename.
+        
+        coloring_method: str, default 'mean'
+        To determine how the color of each residue is produced. Can be 'mean', 
+        where the mean pKa value accross all frames is used or 
+        'difference_to_model_value' where the mean pKa value is calculated 
+        and the difference to the model value of the amino acid in solution is 
+        used. 
+        
+        lower limit: int or float, default 0
+        Determines lower limit used to colour the reisdues in the PyMOL session. Any 
+        value below the limit is coloured using the lowest end of the color gradient 
+        used. 
+        
+        upper limit: int or float, default 14
+        Determines upper limit used to colour the reisdues in the PyMOL session. Any 
+        value above the limit is coloured using the highest end of the color gradient 
+        used. 
+
+        color_palette: str, default 'red_white_blue'
+        color palettes used to color the residues in the PyMOL session according to 
+        the pKa value. The default is set to 'red_white_blue'. See PyMOL spectrum for
+        allowed color palettes. Three colors palette is suggested.
+        """
         u = mda.Universe(self.structure)
         
         #load pKa values and remove time column 
         pka_values = pd.read_csv(self.pka_file) 
         del pka_values['Time [ps]'] 
         
         #calculation of values depending on colouring method 
@@ -87,17 +101,23 @@
                 elif 'C-' in residue: 
                     pka_values_mean[residue] = pka_values_mean[residue]-model_pka_values['CTR'] 
                 else: 
                     pka_values_mean[residue] = pka_values_mean[residue]-model_pka_values[residue[0:3]] 
             pka_values_summary = pka_values_mean
             tempfactors_output_structure = f"{self.pka_file.split('/')[-1].split('.')[0]}_difference_to_model_value.pdb"
         
-        
+        # GROMACS atom naming scheme, other naming scheme will not be valid, user may 
+        # need to add it by themselves for Nterm and Cterm.
         Nterm_atoms = 'N H1 H2 H3'
-        Cterm_atoms = 'C OC1 OC2 OT1 OT2'
+        Cterm_atoms = 'C O OC1 OC2 OT1 OT2 OXT'
+        # Looping the pka_values_summary which contains one column of the name for 
+        # residue and resid, and the other column of predicted pKa. The tempfactor 
+        # (previously known as bfactor) of individual residue is assigned according 
+        # to the predicted pKa from pka_values_summary. The structure with the 
+        # tempfactor is written as pdb and a PyMOL session is generated as pse.
         for residue, predicted_pka in pka_values_summary.items():
             if 'N+' in residue or 'C-' in residue:
                 resid = int(residue[2:])
             else:
                 resid = int(residue[3:])
             rounded_predicted_pka = round(predicted_pka,2)
             if 'N+' in residue:
@@ -110,10 +130,10 @@
                 ag = u.select_atoms(f'resid {resid} and not name {Cterm_atoms}')
             else:
                 ag = u.select_atoms(f'resid {resid}')
             ag.tempfactors = np.full(ag.tempfactors.shape,rounded_predicted_pka)
         ag = u.select_atoms('all')
         ag.write(tempfactors_output_structure)
         pse_output_filename = f'{pse_output_prefix}_{coloring_method}.pse'
-        visualise_pka(tempfactors_output_structure, pymol_path, pse_output_filename, pka_values_summary, lower_limit, upper_limit, color_palette) 
+        visualize_pka(tempfactors_output_structure, pymol_path, pse_output_filename, pka_values_summary, lower_limit, upper_limit, color_palette)
```

### Comparing `tripp-0.1.8/tripp/edit_pdb.py` & `tripp-0.1.9/tripp/edit_pdb.py`

 * *Files identical despite different names*

### Comparing `tripp-0.1.8/tripp/model_pka_values.py` & `tripp-0.1.9/tripp/model_pka_values.py`

 * *Files identical despite different names*

### Comparing `tripp-0.1.8/PKG-INFO` & `tripp-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripp
-Version: 0.1.8
+Version: 0.1.9
 Summary: Trajectory Iterative pKa Predictor
 Author: Christos Matsingos
 Author-email: c.matsingos@qmul.ac.uk>, Ka Fu Man <k.man@qmul.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

