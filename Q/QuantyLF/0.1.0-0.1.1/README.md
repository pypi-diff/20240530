# Comparing `tmp/quantylf-0.1.0.tar.gz` & `tmp/quantylf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantylf-0.1.0.tar", last modified: Mon May 27 16:55:13 2024, max compression
+gzip compressed data, was "quantylf-0.1.1.tar", last modified: Thu May 30 16:14:38 2024, max compression
```

## Comparing `quantylf-0.1.0.tar` & `quantylf-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 16:55:08.000000 quantylf-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-27 16:55:08.000000 quantylf-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-27 16:55:13.040406 quantylf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-27 16:55:08.000000 quantylf-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 16:55:08.000000 quantylf-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 16:55:13.040406 quantylf-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.036406 quantylf-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.036406 quantylf-0.1.0/src/QuantyLF/
--rw-r--r--   0 runner    (1001) docker     (127)    19561 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/QuantyLF.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF/cases/
--rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Td_3d.lua
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/Td_3d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF/cases/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-27 16:55:08.000000 quantylf-0.1.0/src/QuantyLF/cases/utils/slater_integrals.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:55:13.040406 quantylf-0.1.0/src/QuantyLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 16:55:13.000000 quantylf-0.1.0/src/QuantyLF.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.447420 quantylf-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 16:14:34.000000 quantylf-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-30 16:14:34.000000 quantylf-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-30 16:14:38.447420 quantylf-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-05-30 16:14:34.000000 quantylf-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 16:14:34.000000 quantylf-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 16:14:38.447420 quantylf-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.443420 quantylf-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.443420 quantylf-0.1.1/src/QuantyLF/
+-rw-r--r--   0 runner    (1001) docker     (127)    20130 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/QuantyLF.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.443420 quantylf-0.1.1/src/QuantyLF/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/D3h_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/D3h_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/Oh_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/Oh_3d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19083 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/Td_3d.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/Td_3d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.443420 quantylf-0.1.1/src/QuantyLF/cases/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-30 16:14:34.000000 quantylf-0.1.1/src/QuantyLF/cases/utils/slater_integrals.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:14:38.443420 quantylf-0.1.1/src/QuantyLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-30 16:14:38.000000 quantylf-0.1.1/src/QuantyLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 16:14:38.000000 quantylf-0.1.1/src/QuantyLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:14:38.000000 quantylf-0.1.1/src/QuantyLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 16:14:38.000000 quantylf-0.1.1/src/QuantyLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 16:14:38.000000 quantylf-0.1.1/src/QuantyLF.egg-info/top_level.txt
```

### Comparing `quantylf-0.1.0/LICENSE` & `quantylf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantylf-0.1.0/PKG-INFO` & `quantylf-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.1.0
+Version: 0.1.1
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,15 @@
 # create new instance
 quantyLF = QuantyLF()
 # set custom quanty command
 quantyLF.set_quanty_command('../Quanty_macOS', 'Darwin')
 
 # load experimental data including excitation energies
 quantyLF.load_exp_xas('XAS_Exp.dat')
-quantyLF.load_exp_rixs('RIXS_Exp.dat', [638, 639.35])
+quantyLF.load_exp_rixs('RIXS_Exp.dat')
 
 # configure edge jump
 # set display to True to see a plot of experimental data along edge jump (display has to be set to false for calculation)
 quantyLF.config_edge_jump([[637.7, 0.14, 4], [648.2, 0.006, 8]], [600, 700,], display=False)
 
 # see available cases
 print(quantyLF.available_cases())
@@ -300,16 +300,16 @@
 """
 Load the experimental RIXS data from a file (no header, first row: resonance energies, rest of the rows: energy, intensity)
 
 Parameters
 ----------
 path: str   
     Path to the file containing the experimental RIXS data
-RIXS_energies: list of floats
-    List of resonance energies for which the RIXS data is available
+RIXS_energies: list of floats, optional
+    List of resonance energies for which the RIXS data is available (if not provided, the first row of the file is used to extract the resonance energies)
 """
 load_exp_rixs(path, RIXS_energies)
 ```
 
 ### set_quanty_command
 ```py
 """
```

### Comparing `quantylf-0.1.0/README.md` & `quantylf-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # create new instance
 quantyLF = QuantyLF()
 # set custom quanty command
 quantyLF.set_quanty_command('../Quanty_macOS', 'Darwin')
 
 # load experimental data including excitation energies
 quantyLF.load_exp_xas('XAS_Exp.dat')
-quantyLF.load_exp_rixs('RIXS_Exp.dat', [638, 639.35])
+quantyLF.load_exp_rixs('RIXS_Exp.dat')
 
 # configure edge jump
 # set display to True to see a plot of experimental data along edge jump (display has to be set to false for calculation)
 quantyLF.config_edge_jump([[637.7, 0.14, 4], [648.2, 0.006, 8]], [600, 700,], display=False)
 
 # see available cases
 print(quantyLF.available_cases())
@@ -280,16 +280,16 @@
 """
 Load the experimental RIXS data from a file (no header, first row: resonance energies, rest of the rows: energy, intensity)
 
 Parameters
 ----------
 path: str   
     Path to the file containing the experimental RIXS data
-RIXS_energies: list of floats
-    List of resonance energies for which the RIXS data is available
+RIXS_energies: list of floats, optional
+    List of resonance energies for which the RIXS data is available (if not provided, the first row of the file is used to extract the resonance energies)
 """
 load_exp_rixs(path, RIXS_energies)
 ```
 
 ### set_quanty_command
 ```py
 """
```

### Comparing `quantylf-0.1.0/setup.cfg` & `quantylf-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QuantyLF
-version = 0.1.0
+version = 0.1.1
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `quantylf-0.1.0/src/QuantyLF/QuantyLF.py` & `quantylf-0.1.1/src/QuantyLF/QuantyLF.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,26 +463,33 @@
     """
     Load the experimental RIXS data from a file (no header, first row: resonance energies, rest of the rows: energy, intensity)
 
     Parameters
     ----------
     path: str   
         Path to the file containing the experimental RIXS data
-    RIXS_energies: list of floats
-        List of resonance energies for which the RIXS data is available
+    RIXS_energies: list of floats, optional
+        List of resonance energies for which the RIXS data is available (if not provided, the first row of the file is used to extract the resonance energies)
     """
-    def load_exp_rixs(self, path, RIXS_energies):        
+    def load_exp_rixs(self, path, RIXS_energies=None):        
         #load exp RIXS. For experimental, the first row are the resonance energies
         expRIXS = np.loadtxt(path)
         energies = expRIXS[0,:]
         if energies[0] != 0:
-            raise ValueError("First value of the first row should be 0, as it is the energy axis for the RIXS data")
-        for i in range(len(RIXS_energies)):
-            if RIXS_energies[i] != energies[i+1]:
-                raise ValueError(f"Resonant energy {RIXS_energies[i]} not found in the experimental RIXS data. First row should contain the resonance energies")
+            raise ValueError("First value of the first row should be 0, as it is the energy axis for the RIXS data")        
+        if RIXS_energies is None:
+            RIXS_energies = energies[1:]
+        else:
+            # check if number rixs energies is equal to number of columns in expRIXS
+            if len(RIXS_energies) != len(expRIXS[1,:])-1:
+                raise ValueError("Number of RIXS energies does not match the number of columns in the experimental RIXS data")
+            # check if the rixs energies match energies in the first row of the expRIXS
+            for i in range(len(RIXS_energies)):
+                if RIXS_energies[i] != energies[i+1]:
+                    raise ValueError(f"Resonant energy {RIXS_energies[i]} not found in the experimental RIXS data. First row should contain the resonance energies")
 
         for RIXS_energy in RIXS_energies:
             self.add_par("RIXS",RIXS_energy,from_file=False)
         
         #trim the exp RIXS just to have the columns with resonant energies we are calculating
         indices = [0] #0th column is energy, which we will keep
         for i in range(len(RIXS_energies)):
```

### Comparing `quantylf-0.1.0/src/QuantyLF/cases/D3h_3d.lua` & `quantylf-0.1.1/src/QuantyLF/cases/D3h_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.1.0/src/QuantyLF/cases/Oh_3d.lua` & `quantylf-0.1.1/src/QuantyLF/cases/Oh_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.1.0/src/QuantyLF/cases/Td_3d.lua` & `quantylf-0.1.1/src/QuantyLF/cases/Td_3d.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.1.0/src/QuantyLF/cases/utils/slater_integrals.lua` & `quantylf-0.1.1/src/QuantyLF/cases/utils/slater_integrals.lua`

 * *Files identical despite different names*

### Comparing `quantylf-0.1.0/src/QuantyLF.egg-info/PKG-INFO` & `quantylf-0.1.1/src/QuantyLF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantyLF
-Version: 0.1.0
+Version: 0.1.1
 Summary: QuantyLF is a libary to help manage Liegand Field simulations in Quanty.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,15 @@
 # create new instance
 quantyLF = QuantyLF()
 # set custom quanty command
 quantyLF.set_quanty_command('../Quanty_macOS', 'Darwin')
 
 # load experimental data including excitation energies
 quantyLF.load_exp_xas('XAS_Exp.dat')
-quantyLF.load_exp_rixs('RIXS_Exp.dat', [638, 639.35])
+quantyLF.load_exp_rixs('RIXS_Exp.dat')
 
 # configure edge jump
 # set display to True to see a plot of experimental data along edge jump (display has to be set to false for calculation)
 quantyLF.config_edge_jump([[637.7, 0.14, 4], [648.2, 0.006, 8]], [600, 700,], display=False)
 
 # see available cases
 print(quantyLF.available_cases())
@@ -300,16 +300,16 @@
 """
 Load the experimental RIXS data from a file (no header, first row: resonance energies, rest of the rows: energy, intensity)
 
 Parameters
 ----------
 path: str   
     Path to the file containing the experimental RIXS data
-RIXS_energies: list of floats
-    List of resonance energies for which the RIXS data is available
+RIXS_energies: list of floats, optional
+    List of resonance energies for which the RIXS data is available (if not provided, the first row of the file is used to extract the resonance energies)
 """
 load_exp_rixs(path, RIXS_energies)
 ```
 
 ### set_quanty_command
 ```py
 """
```

