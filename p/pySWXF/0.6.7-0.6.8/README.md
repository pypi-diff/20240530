# Comparing `tmp/pyswxf-0.6.7.tar.gz` & `tmp/pyswxf-0.6.8.tar.gz`

## Comparing `pyswxf-0.6.7.tar` & `pyswxf-0.6.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.7/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.7/cbwe.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.7/dot_pypirc
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.7/instructions
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.7/pyproject.bak
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.7/pyproject.new
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.7/token
--rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
--rwxr-xr-x   0        0        0    14262 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/AuI_funs.py
--rwxr-xr-x   0        0        0     2479 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/Br_funs.py
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/__init__.py
--rwxr-xr-x   0        0        0     8356 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/fluor_fit.py
--rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
--rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/refl_funs.py
--rwxr-xr-x   0        0        0    27347 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/spec_utils.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/view_new_multilayer.ipynb
--rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.7/src/pySWXF/xray_utils.py
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.7/LICENSE
--rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.7/README.md
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.7/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.8/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.8/cbwe.py
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.8/dot_pypirc
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.8/instructions
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.bak
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.new
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.8/token
+-rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
+-rwxr-xr-x   0        0        0    21877 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/AuI_funs.py
+-rwxr-xr-x   0        0        0     2479 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/Br_funs.py
+-rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/__init__.py
+-rwxr-xr-x   0        0        0    12009 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/fluor_fit.py
+-rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
+-rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/refl_funs.py
+-rwxr-xr-x   0        0        0    27347 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/spec_utils.py
+-rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/view_new_multilayer.ipynb
+-rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.8/src/pySWXF/xray_utils.py
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.8/LICENSE
+-rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.8/README.md
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.8/PKG-INFO
```

### Comparing `pyswxf-0.6.7/dot_pypirc` & `pyswxf-0.6.8/dot_pypirc`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/pyproject.bak` & `pyswxf-0.6.8/pyproject.bak`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/pyproject.new` & `pyswxf-0.6.8/pyproject.new`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py` & `pyswxf-0.6.8/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/Br_funs.py` & `pyswxf-0.6.8/src/pySWXF/Br_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json` & `pyswxf-0.6.8/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/fluor_fit.py` & `pyswxf-0.6.8/src/pySWXF/fluor_fit.py`

 * *Files 24% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         layers += [('Mo',rMo,D*G,sig_Mo),
                        ('Si',rSi,D*(1-G),sig_Si)]
     layers += [('Ti',xdb.atomic_density('Ti'),D_Ti,sig_Ti), 
                    ('SiO2',2.2,D_SiO2_Bot,sig_SiO2_Bot),
                    ('Si',xdb.atomic_density('Si'),0,sig_Si_Bot)]
     return layers
 
-def multilayer_ref_Ti(theta,I0,thoff,
+def multilayer_ref_Ti_orig(theta,I0,thoff,
                    bg,foot,G,D,sig_Mo,sig_Si,overlay,
                    sig_Si_top,water,
                    Energy,bilayer,res,D_Ti,sig_Ti,D_SiO2,sig_SiO2,
                    D_SiO2_Bot,sig_SiO2_Bot,sig_Si_Bot):
     if res == 0:
         norm = 1
         nspan = 1
@@ -103,14 +103,77 @@
         Intensity[frange] *= theta[frange]/foot
         tres = Intensity*mul[i]/norm
         result_list.append(tres)       
     toc = time.time()
     #print(f'{toc-tic:2.1f} ',end='')
     return(I0*np.sum(np.array(result_list),0)+bg)
 
+import numpy as np
+import scipy.constants as scc
+import scipy.signal as scs
+
+def multilayer_ref_Ti(
+    theta: np.ndarray,
+    I0: float,
+    thoff: float,
+    bg: float,
+    foot: float,
+    G: float,
+    D: float,
+    sig_Mo: float,
+    sig_Si: float,
+    overlay: float,
+    sig_Si_top: float,
+    water: bool,
+    Energy: float,
+    bilayer: bool,
+    res: float,
+    D_Ti: float,
+    sig_Ti: float,
+    D_SiO2: float,
+    sig_SiO2: float,
+    D_SiO2_Bot: float,
+    sig_SiO2_Bot: float,
+    sig_Si_Bot: float
+) -> np.ndarray:
+    theta = np.array(theta)
+    theta_off = theta - thoff
+    
+    # Recast data on uniform grid
+    dth = np.min(np.diff(theta_off))
+    npt = int((theta_off[-1] - theta_off[0]) / dth)
+    thnew = np.linspace(theta_off[0], theta_off[-1], npt)
+    
+    # Simulate sample layers
+    layers = sample_sim(G, D, sig_Mo, sig_Si, overlay, sig_Si_top, water, bilayer,
+                        D_Ti=D_Ti, sig_Ti=sig_Ti, D_SiO2=D_SiO2, sig_SiO2=sig_SiO2,
+                        D_SiO2_Bot=D_SiO2_Bot, sig_SiO2_Bot=sig_SiO2_Bot, sig_Si_Bot=sig_Si_Bot)
+    alpha = thnew * scc.degree
+    
+    # Compute reflection matrix
+    _, r, _, _, _, _, _ = reflection_matrix(alpha, Energy, layers)
+    Intensity = np.abs(r[:, 0])**2
+    
+    # Correct for footprint
+    frange = thnew < foot
+    Intensity[frange] *= thnew[frange] / foot
+    
+    # Include resolution using convolution
+    if res > 0:
+        signal = np.concatenate([Intensity[::-1], Intensity, Intensity[::-1]])
+        sig = res / dth
+        nwin = 8 * int(sig) + 16
+        win = np.exp(-0.5 * (np.arange(-nwin // 2, nwin // 2 + 1) / sig)**2)
+        win /= win.sum()
+        Intensity = scs.convolve(signal, win, mode='same')[npt:2*npt]
+    
+    # Re-interpolate data back to old angles
+    Iout = np.interp(theta_off, thnew, Intensity)
+    return I0 * Iout + bg
+
 
 def multilayer_fluor(theta,I0,thoff,
                    bg,foot,G,D,sig_Mo,sig_Si,overlay,
                    sig_Si_top,sep,hoff,res,
                    Energy):
     water = True
     bilayer = True 
@@ -189,15 +252,15 @@
     layers += [(Cr.formula,Cr.density,D_Cr,sig_Cr)]
     # add substrate
     layers += [(Si.formula,Si.density,0,sig_Si_Bot)]
     return layers
 
 
 
-def multilayer_ref_new(theta,I0,thoff,bg,foot,G,D,d_overlay, sig_overlay,
+def multilayer_ref_new_orig(theta,I0,thoff,bg,foot,G,D,d_overlay, sig_overlay,
     sig_W,sig_SiC,Energy,res,D_Cr,sig_Cr,sig_Si_Bot, water=True,bilayer=True, new_cell=True):
     theta = np.array(theta)
     theta_off = theta - thoff
     #recast data on uniform grid
     dth = min(theta_off[1:]-theta_off[0:-1])
     npt = int((theta_off[-1]-theta_off[0])/dth)
     thnew = np.linspace(theta_off[0],theta_off[-1],npt)
@@ -222,13 +285,73 @@
         signal2 = scs.convolve(signal,win,mode='same')
         signal2 = signal2[npt:2*npt]
         Intensity = signal2
     # re-interpolate data back to old angles
     Iout = np.interp(theta_off,thnew,Intensity)
     return(I0*Iout+bg)
 
+import numpy as np
+import scipy.constants as scc
+import scipy.signal as scs
+
+
+
+def multilayer_ref_new(
+    theta: np.ndarray,
+    I0: float,
+    thoff: float,
+    bg: float,
+    foot: float,
+    G: float,
+    D: float,
+    d_overlay: float,
+    sig_overlay: float,
+    sig_W: float,
+    sig_SiC: float,
+    Energy: float,
+    res: float,
+    D_Cr: float,
+    sig_Cr: float,
+    sig_Si_Bot: float,
+    water: bool = True,
+    bilayer: bool = True,
+    new_cell: bool = True
+) -> np.ndarray:
+    theta = np.array(theta)
+    theta_off = theta - thoff
+    
+    # Recast data on uniform grid
+    dth = np.min(np.diff(theta_off))
+    npt = int((theta_off[-1] - theta_off[0]) / dth)
+    thnew = np.linspace(theta_off[0], theta_off[-1], npt)
+    
+    # Simulate sample layers
+    layers = sample_sim_new(d_overlay, sig_overlay, G, D, sig_W, sig_SiC, D_Cr, sig_Cr, sig_Si_Bot, water=water, bilayer=bilayer, new_cell=new_cell)
+    alpha = thnew * scc.degree
+    
+    # Compute reflection matrix
+    _, r, _, _, _, _, _ = reflection_matrix(alpha, Energy, layers)
+    Intensity = np.abs(r[:, 0])**2
+    
+    # Correct for footprint
+    frange = thnew < foot
+    Intensity[frange] *= thnew[frange] / foot
+    
+    # Include resolution
+    if res > 0:
+        signal = np.concatenate([Intensity[::-1], Intensity, Intensity[::-1]])
+        sig = res / dth
+        nwin = 8 * int(sig) + 16
+        win = np.exp(-0.5 * (np.arange(-nwin // 2, nwin // 2 + 1) / sig)**2)
+        win /= win.sum()
+        Intensity = scs.convolve(signal, win, mode='same')[npt:2*npt]
+    
+    # Re-interpolate data back to old angles
+    Iout = np.interp(theta_off, thnew, Intensity)
+    return I0 * Iout + bg
+
 
 multilayer_ref_new_model = Model(multilayer_ref_new,
     independent_vars = ['theta','Energy','water','bilayer','new_cell'])
```

### Comparing `pyswxf-0.6.7/src/pySWXF/niu_multilayer_fit_params_3_LBL.json` & `pyswxf-0.6.8/src/pySWXF/niu_multilayer_fit_params_3_LBL.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/refl_funs.py` & `pyswxf-0.6.8/src/pySWXF/refl_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/spec_utils.py` & `pyswxf-0.6.8/src/pySWXF/spec_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/view_new_multilayer.ipynb` & `pyswxf-0.6.8/src/pySWXF/view_new_multilayer.ipynb`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/src/pySWXF/xray_utils.py` & `pyswxf-0.6.8/src/pySWXF/xray_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/LICENSE` & `pyswxf-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/README.md` & `pyswxf-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.7/pyproject.toml` & `pyswxf-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling==1.17.1"]
 build-backend = "hatchling.build"
 [project]
 name = "pySWXF"
-version = "0.6.7"
+version = "0.6.8"
 authors = [
 	{name="Laurence Lurio", email="llurio@niu.edu" },
 ]
 description = "Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `pyswxf-0.6.7/PKG-INFO` & `pyswxf-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySWXF
-Version: 0.6.7
+Version: 0.6.8
 Summary: Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity
 Project-URL: Homepage, https://github.com/pypa/pySWXF
 Project-URL: Bug Tracker, https://github.com/pypa/pySWXF/issues
 Author-email: Laurence Lurio <llurio@niu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

