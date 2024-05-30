# Comparing `tmp/damask-3.0.0b0.tar.gz` & `tmp/damask-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damask-3.0.0b0.tar", last modified: Tue Jan 23 14:29:38 2024, max compression
+gzip compressed data, was "damask-3.0.0b2.tar", last modified: Thu May 30 17:25:27 2024, max compression
```

## Comparing `damask-3.0.0b0.tar` & `damask-3.0.0b2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-01-23 14:29:38.662404 damask-3.0.0b0/
--rw-r--r--   0 m         (1000) m         (1000)       46 2024-01-23 14:20:43.000000 damask-3.0.0b0/MANIFEST.in
--rw-r--r--   0 m         (1000) m         (1000)      726 2024-01-23 14:29:38.662404 damask-3.0.0b0/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)     1201 2024-01-23 14:20:43.000000 damask-3.0.0b0/README.md
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-01-23 14:29:38.662404 damask-3.0.0b0/damask/
--rw-r--r--   0 m         (1000) m         (1000)      694 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/LICENSE
--rw-r--r--   0 m         (1000) m         (1000)        8 2024-01-23 14:29:36.000000 damask-3.0.0b0/damask/VERSION
--rw-r--r--   0 m         (1000) m         (1000)     2130 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)    25460 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_colormap.py
--rw-r--r--   0 m         (1000) m         (1000)    24394 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_configmaterial.py
--rw-r--r--   0 m         (1000) m         (1000)    52746 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_crystal.py
--rw-r--r--   0 m         (1000) m         (1000)    59327 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_geomgrid.py
--rw-r--r--   0 m         (1000) m         (1000)     3315 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_loadcasegrid.py
--rw-r--r--   0 m         (1000) m         (1000)    36472 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_orientation.py
--rw-r--r--   0 m         (1000) m         (1000)    93061 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_result.py
--rw-r--r--   0 m         (1000) m         (1000)    73231 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_rotation.py
--rw-r--r--   0 m         (1000) m         (1000)    19371 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_table.py
--rw-r--r--   0 m         (1000) m         (1000)     1955 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_typehints.py
--rw-r--r--   0 m         (1000) m         (1000)    22863 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_vtk.py
--rw-r--r--   0 m         (1000) m         (1000)     7568 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/_yaml.py
--rw-r--r--   0 m         (1000) m         (1000)    21197 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/grid_filters.py
--rw-r--r--   0 m         (1000) m         (1000)     9835 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/mechanics.py
--rw-r--r--   0 m         (1000) m         (1000)     7512 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/seeds.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-01-23 14:29:38.662404 damask-3.0.0b0/damask/solver/
--rw-r--r--   0 m         (1000) m         (1000)      808 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/solver/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     4091 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/solver/_marc.py
--rw-r--r--   0 m         (1000) m         (1000)     3699 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/tensor.py
--rw-r--r--   0 m         (1000) m         (1000)    34144 2024-01-23 14:20:43.000000 damask-3.0.0b0/damask/util.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-01-23 14:29:38.662404 damask-3.0.0b0/damask.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)      726 2024-01-23 14:29:38.000000 damask-3.0.0b0/damask.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)      623 2024-01-23 14:29:38.000000 damask-3.0.0b0/damask.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2024-01-23 14:29:38.000000 damask-3.0.0b0/damask.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)       84 2024-01-23 14:29:38.000000 damask-3.0.0b0/damask.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)        7 2024-01-23 14:29:38.000000 damask-3.0.0b0/damask.egg-info/top_level.txt
--rw-r--r--   0 m         (1000) m         (1000)      100 2024-01-23 14:20:43.000000 damask-3.0.0b0/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)     1147 2024-01-23 14:29:38.662404 damask-3.0.0b0/setup.cfg
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-30 17:25:27.748238 damask-3.0.0b2/
+-rw-r--r--   0 m         (1000) m         (1000)       46 2024-05-30 05:32:01.000000 damask-3.0.0b2/MANIFEST.in
+-rw-r--r--   0 m         (1000) m         (1000)      726 2024-05-30 17:25:27.748238 damask-3.0.0b2/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)     1203 2024-05-30 05:32:02.000000 damask-3.0.0b2/README.md
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-30 17:25:27.748238 damask-3.0.0b2/damask/
+-rw-r--r--   0 m         (1000) m         (1000)      694 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/LICENSE
+-rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-30 17:25:24.000000 damask-3.0.0b2/damask/VERSION
+-rw-r--r--   0 m         (1000) m         (1000)     2130 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)    25815 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_colormap.py
+-rw-r--r--   0 m         (1000) m         (1000)    24126 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_configmaterial.py
+-rw-r--r--   0 m         (1000) m         (1000)    53017 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_crystal.py
+-rw-r--r--   0 m         (1000) m         (1000)    60013 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_geomgrid.py
+-rw-r--r--   0 m         (1000) m         (1000)     3315 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_loadcasegrid.py
+-rw-r--r--   0 m         (1000) m         (1000)    38595 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_orientation.py
+-rw-r--r--   0 m         (1000) m         (1000)    93966 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_result.py
+-rw-r--r--   0 m         (1000) m         (1000)    73303 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_rotation.py
+-rw-r--r--   0 m         (1000) m         (1000)    19371 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_table.py
+-rw-r--r--   0 m         (1000) m         (1000)     1955 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_typehints.py
+-rw-r--r--   0 m         (1000) m         (1000)    22863 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_vtk.py
+-rw-r--r--   0 m         (1000) m         (1000)     7558 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/_yaml.py
+-rw-r--r--   0 m         (1000) m         (1000)    21197 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/grid_filters.py
+-rw-r--r--   0 m         (1000) m         (1000)     9842 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/mechanics.py
+-rw-r--r--   0 m         (1000) m         (1000)     7512 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/seeds.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-30 17:25:27.748238 damask-3.0.0b2/damask/solver/
+-rw-r--r--   0 m         (1000) m         (1000)      808 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/solver/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)     4091 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/solver/_marc.py
+-rw-r--r--   0 m         (1000) m         (1000)     3699 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/tensor.py
+-rw-r--r--   0 m         (1000) m         (1000)    34421 2024-05-30 05:32:01.000000 damask-3.0.0b2/damask/util.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-30 17:25:27.748238 damask-3.0.0b2/damask.egg-info/
+-rw-r--r--   0 m         (1000) m         (1000)      726 2024-05-30 17:25:27.000000 damask-3.0.0b2/damask.egg-info/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)      623 2024-05-30 17:25:27.000000 damask-3.0.0b2/damask.egg-info/SOURCES.txt
+-rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-30 17:25:27.000000 damask-3.0.0b2/damask.egg-info/dependency_links.txt
+-rw-r--r--   0 m         (1000) m         (1000)       84 2024-05-30 17:25:27.000000 damask-3.0.0b2/damask.egg-info/requires.txt
+-rw-r--r--   0 m         (1000) m         (1000)        7 2024-05-30 17:25:27.000000 damask-3.0.0b2/damask.egg-info/top_level.txt
+-rw-r--r--   0 m         (1000) m         (1000)      100 2024-05-30 05:32:01.000000 damask-3.0.0b2/pyproject.toml
+-rw-r--r--   0 m         (1000) m         (1000)     1147 2024-05-30 17:25:27.751572 damask-3.0.0b2/setup.cfg
```

### Comparing `damask-3.0.0b0/PKG-INFO` & `damask-3.0.0b2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damask
-Version: 3.0.0b0
+Version: 3.0.0b2
 Summary: DAMASK processing tools
 Home-page: https://damask.mpie.de
 Author: The DAMASK team
 Author-email: damask@mpie.de
 License: AGPL3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `damask-3.0.0b0/README.md` & `damask-3.0.0b2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 Max-Planck-Institut für Eisenforschung GmbH  
 Max-Planck-Str. 1  
 40237 Düsseldorf  
 Germany  
 
 ## Version Information
 
-Revision v3.0.0-beta  
-Exported on Tue 23 Jan 2024 15:20:43 CET  
+Revision v3.0.0-beta2  
+Exported on Thu 30 May 2024 07:32:02 CEST
```

### Comparing `damask-3.0.0b0/damask/LICENSE` & `damask-3.0.0b2/damask/LICENSE`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/__init__.py` & `damask-3.0.0b2/damask/__init__.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/_colormap.py` & `damask-3.0.0b2/damask/_colormap.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,48 +57,67 @@
     https://doi.org/10.1016/j.ijplas.2012.09.012
 
     Matplotlib colormaps overview
     https://matplotlib.org/stable/tutorials/colors/colormaps.html
 
     """
 
+    def __init__(self,
+                 colors: np.ndarray, name: str):
+        """
+        New colormap.
+
+        Parameters
+        ----------
+        colors : numpy.ndarray, shape (:,3) or (:,4)
+            Color specifications as RGB(A) values.
+        name : str
+            String to identify the colormap.
+
+        """
+        super().__init__(colors,name)
+        self.colors: np.ndarray = np.asarray(colors)
+
+
     def __eq__(self,
                other: object) -> bool:
         """
         Return self==other.
 
         Test equality of other.
 
         """
         if not isinstance(other, Colormap):
             return NotImplemented
-        return         len(self.colors) == len(other.colors) \
-           and bool(np.all(self.colors  ==     other.colors))
+        return np.array_equal(self.colors,other.colors)
+
 
     def __add__(self,
                 other: 'Colormap') -> 'Colormap':
         """
         Return self+other.
 
         Concatenate.
 
         """
         return Colormap(np.vstack((self.colors,other.colors)),
                         f'{self.name}+{other.name}')
 
+
     def __iadd__(self,
                  other: 'Colormap') -> 'Colormap':
         """
         Return self+=other.
 
         Concatenate (in-place).
 
         """
         return self.__add__(other)
 
+
     def __mul__(self,
                 factor: int) -> 'Colormap':
         """
         Return self*other.
 
         Repeat.
 
@@ -111,32 +130,34 @@
         Return self*=other.
 
         Repeat (in-place).
 
         """
         return self.__mul__(factor)
 
+
     def __invert__(self) -> 'Colormap':
         """
         Return ~self.
 
         Reverse.
 
         """
         return self.reversed()
 
+
     def __repr__(self) -> str:
         """
         Return repr(self).
 
         Show as matplotlib figure.
 
         """
         fig = plt.figure(self.name,figsize=(5,.5))
-        ax1 = fig.add_axes([0, 0, 1, 1])
+        ax1 = fig.add_axes((0, 0, 1, 1))
         ax1.set_axis_off()
         ax1.imshow(np.linspace(0,1,self.N).reshape(1,-1),
                    aspect='auto', cmap=self, interpolation='nearest')
         plt.show(block=False)
         return f'Colormap: {self.name}'
```

### Comparing `damask-3.0.0b0/damask/_configmaterial.py` & `damask-3.0.0b2/damask/_configmaterial.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from typing import Optional, Union, Sequence, Dict, Any, List
 
 import numpy as np
 import h5py
 
-from ._typehints import FileHandle, FloatSequence, StrSequence
+from ._typehints import FloatSequence, StrSequence
 from . import YAML
 from . import Rotation
 from . import Orientation
 from . import util
 from . import tensor
 from . import Table
 
 
 class ConfigMaterial(YAML):
     """
     Material configuration.
 
     Manipulate material configurations for storage in YAML format.
     A complete material configuration file has the entries 'material',
-    'phase', and 'homogenization'. For use in DAMASK, it needs to be
-    stored as 'material.yaml'.
+    'phase', and 'homogenization'.
 
     """
 
     def __init__(self,
                  config: Optional[Union[str,Dict[str,Any]]] = None,*,
                  homogenization: Optional[Dict[str,Dict]] = None,
                  phase: Optional[Dict[str,Dict]] = None,
@@ -66,51 +65,14 @@
                 kwargs[arg] = [] if arg == 'material' else {}
             elif value is not None:
                 kwargs[arg] = value
 
         super().__init__(config,**kwargs)
 
 
-    def save(self,
-             fname: FileHandle = 'material.yaml',
-             **kwargs):
-        """
-        Save to YAML file.
-
-        Parameters
-        ----------
-        fname : file, str, or pathlib.Path, optional
-            Filename or file for writing. Defaults to 'material.yaml'.
-        **kwargs
-            Keyword arguments parsed to yaml.dump.
-
-        """
-        super().save(fname,**kwargs)
-
-
-    @classmethod
-    def load(cls,
-             fname: FileHandle = 'material.yaml') -> 'ConfigMaterial':
-        """
-        Load from YAML file.
-
-        Parameters
-        ----------
-        fname : file, str, or pathlib.Path, optional
-            Filename or file to read from. Defaults to 'material.yaml'.
-
-        Returns
-        -------
-        loaded : damask.ConfigMaterial
-            Material configuration from file.
-
-        """
-        return super(ConfigMaterial,cls).load(fname)
-
-
     @staticmethod
     def load_DREAM3D(fname: str,
                      grain_data: Optional[str] = None,
                      cell_data: Optional[str] = None,
                      cell_ensemble_data: str = 'CellEnsembleData',
                      phases: str = 'Phases',
                      Euler_angles: str = 'EulerAngles',
@@ -154,19 +116,28 @@
         Returns
         -------
         loaded : damask.ConfigMaterial
             Material configuration from file.
 
         Notes
         -----
-        damask.GeomGrid.load_DREAM3D gives the corresponding geometry for
-        the grid solver.
-
-        For cell-wise data, only unique combinations of
-        orientation and phase are considered.
+        A grain-wise material configuration is based on segmented data from
+        the DREAM.3D file. This data is typically available when the microstructure
+        was synthetically created. In cell-wise representations, cells having the
+        same orientation and phase are grouped. Since synthetically created
+        microstructures have typically no in-grain scatter, cell-wise grids
+        can appear to be segmented.
+
+        damask.GeomGrid.load_DREAM3D creates the corresponding grid-based
+        geometry definition. Since the numbering of materials in cell-wise
+        and grain-wise grids is different, it is imperative to use the same
+        mode for both load_DREAM3D functions. That means, if the "grain_data"
+        argument is used for this function, the correct grid configuration
+        is only obtained if the "feature_IDs" argument is used when calling
+        damask.GeomGrid.load_DREAM3D.
 
         Homogenization and phase entries are emtpy and need to be
         defined separately.
 
         """
         with h5py.File(fname, 'r') as f:
             b = util.DREAM3D_base_group(f) if base_group is None else base_group
```

### Comparing `damask-3.0.0b0/damask/_crystal.py` & `damask-3.0.0b2/damask/_crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,16 +552,18 @@
         Give short, human-readable summary.
 
         """
         family = f'Crystal family: {self.family}'
         return family if self.lattice is None else \
                util.srepr([family,
                            f'Bravais lattice: {self.lattice}',
-                           'a={:.5g} m, b={:.5g} m, c={:.5g} m'.format(*self.parameters[:3]),
-                           'α={:.5g}°, β={:.5g}°, γ={:.5g}°'.format(*np.degrees(self.parameters[3:]))])
+                           'a={a:.5g} m, b={b:.5g} m, c={c:.5g} m'.format(**self.parameters),
+                           'α={alpha:.5g}°, β={beta:.5g}°, γ={gamma:.5g}°'
+                           .format(**dict(map(lambda kv: (kv[0], np.degrees(kv[1])), self.parameters.items()))),
+                           ])
 
 
     def __eq__(self,
                other: object) -> bool:
         """
         Return self==other.
 
@@ -575,17 +577,18 @@
         """
         return (NotImplemented if not isinstance(other, Crystal) else
                 self.lattice == other.lattice and
                 self.parameters == other.parameters and
                 self.family == other.family)                                                        # type: ignore
 
     @property
-    def parameters(self) -> Optional[Tuple]:
+    def parameters(self) -> Optional[Dict]:
         """Return lattice parameters a, b, c, alpha, beta, gamma."""
-        return (self.a,self.b,self.c,self.alpha,self.beta,self.gamma) if hasattr(self,'a') else None
+        return dict(a=self.a,b=self.b,c=self.c,
+                    alpha=self.alpha,beta=self.beta,gamma=self.gamma) if hasattr(self,'a') else None
 
     @property
     def immutable(self) -> Dict[str, float]:
         """Return immutable lattice parameters."""
         _immutable: Dict[CrystalFamily, Dict[str,float]] = {
             'cubic': {
                          'b': 1.0,
@@ -859,17 +862,17 @@
         Miller : numpy.ndarray, shape (...,3)
             Lattice vector of direction or plane.
             Use util.scale_to_coprime to convert to (integer) Miller indices.
 
         """
         if (direction is not None) ^ (plane is None):
             raise KeyError('specify either "direction" or "plane"')
-        basis,axis = (self.basis_reciprocal,np.array(direction)) \
+        basis,axis = (self.basis_reciprocal,np.asarray(direction)) \
                      if plane is None else \
-                     (self.basis_real,np.array(plane))
+                     (self.basis_real,np.asarray(plane))
         return np.einsum('li,...l',basis,axis)
 
 
     def to_frame(self, *,
                  uvw: Optional[FloatSequence] = None,
                  hkl: Optional[FloatSequence] = None) -> np.ndarray:
         """
@@ -901,17 +904,17 @@
         >>> Ti = damask.Crystal(lattice='hP', a=295e-12, c=469e-12)
         >>> Ti.to_frame(hkl=(1, 0, 0))
         array([ 3.38983051e+09,  1.95711956e+09, -4.15134508e-07])
 
         """
         if (uvw is not None) ^ (hkl is None):
             raise KeyError('specify either "uvw" or "hkl"')
-        basis,axis = (self.basis_real,np.array(uvw)) \
+        basis,axis = (self.basis_real,np.asarray(uvw)) \
                      if hkl is None else \
-                     (self.basis_reciprocal,np.array(hkl))
+                     (self.basis_reciprocal,np.asarray(hkl))
         return np.einsum('il,...l',basis,axis)
 
 
     def kinematics(self,
                    mode: CrystalKinematics) -> Dict[str, List[np.ndarray]]:
         """
         Return crystal kinematics systems.
@@ -961,77 +964,77 @@
                            [ 1,-1, 2,  1,-1,-1],
                            [ 2, 1,-1, -1, 1,-1],
                            [-1,-2,-1, -1, 1,-1],
                            [-1, 1, 2, -1, 1,-1]])]
             },
             'cI': {
                 'slip': [np.array([
-                           [+1,-1,+1,  0,+1,+1],
-                           [-1,-1,+1,  0,-1,-1],
-                           [+1,+1,+1,  0,+1,-1],
-                           [-1,+1,+1,  0,-1,+1],
-                           [-1,+1,+1, -1, 0,-1],
-                           [-1,-1,+1, +1, 0,+1],
-                           [+1,+1,+1, -1, 0,+1],
-                           [+1,-1,+1, +1, 0,-1],
-                           [-1,+1,+1, +1,+1, 0],
-                           [+1,-1,+1, -1,-1, 0],
-                           [+1,+1,+1, +1,-1, 0],
-                           [-1,-1,+1, -1,+1, 0]]),
+                           [+1,-1,+1, +0,+1,+1],
+                           [+1,-1,+1, +1,+0,-1],
+                           [+1,-1,+1, -1,-1,+0],
+                           [-1,-1,+1, +0,-1,-1],
+                           [-1,-1,+1, +1,+0,+1],
+                           [-1,-1,+1, -1,+1,+0],
+                           [+1,+1,+1, +0,+1,-1],
+                           [+1,+1,+1, -1,+0,+1],
+                           [+1,+1,+1, +1,-1,+0],
+                           [-1,+1,+1, +0,-1,+1],
+                           [-1,+1,+1, -1,+0,-1],
+                           [-1,+1,+1, +1,+1,+0]]),
                          np.array([
-                           [-1,+1,+1, +2,+1,+1],
-                           [+1,+1,+1, -2,+1,+1],
-                           [+1,+1,-1, +2,-1,+1],
                            [+1,-1,+1, +2,+1,-1],
+                           [+1,-1,+1, -1,+1,+2],
                            [+1,-1,+1, +1,+2,+1],
-                           [+1,+1,-1, -1,+2,+1],
+                           [-1,-1,+1, +2,-1,+1],
+                           [-1,-1,+1, +1,+1,+2],
+                           [-1,-1,+1, -1,+2,+1],
+                           [+1,+1,+1, +1,+1,-2],
                            [+1,+1,+1, +1,-2,+1],
-                           [-1,+1,+1, +1,+2,-1],
-                           [+1,+1,-1, +1,+1,+2],
-                           [+1,-1,+1, -1,+1,+2],
+                           [+1,+1,+1, -2,+1,+1],
                            [-1,+1,+1, +1,-1,+2],
-                           [+1,+1,+1, +1,+1,-2]]),
+                           [-1,+1,+1, +1,+2,-1],
+                           [-1,+1,+1, +2,+1,+1]]),
                          np.array([
-                           [+1,+1,-1, +1,+2,+3],
                            [+1,-1,+1, -1,+2,+3],
-                           [-1,+1,+1, +1,-2,+3],
-                           [+1,+1,+1, +1,+2,-3],
                            [+1,-1,+1, +1,+3,+2],
-                           [+1,+1,-1, -1,+3,+2],
-                           [+1,+1,+1, +1,-3,+2],
-                           [-1,+1,+1, +1,+3,-2],
-                           [+1,+1,-1, +2,+1,+3],
                            [+1,-1,+1, -2,+1,+3],
-                           [-1,+1,+1, +2,-1,+3],
-                           [+1,+1,+1, +2,+1,-3],
                            [+1,-1,+1, +2,+3,+1],
-                           [+1,+1,-1, -2,+3,+1],
+                           [+1,-1,+1, +3,+1,-2],
+                           [+1,-1,+1, +3,+2,-1],
+                           [-1,-1,+1, +1,+2,+3],
+                           [-1,-1,+1, -1,+3,+2],
+                           [-1,-1,+1, +2,+1,+3],
+                           [-1,-1,+1, -2,+3,+1],
+                           [-1,-1,+1, +3,-1,+2],
+                           [-1,-1,+1, +3,-2,+1],
+                           [+1,+1,+1, +1,+2,-3],
+                           [+1,+1,+1, +1,-3,+2],
+                           [+1,+1,+1, +2,+1,-3],
                            [+1,+1,+1, +2,-3,+1],
-                           [-1,+1,+1, +2,+3,-1],
-                           [-1,+1,+1, +3,+1,+2],
                            [+1,+1,+1, -3,+1,+2],
-                           [+1,+1,-1, +3,-1,+2],
-                           [+1,-1,+1, +3,+1,-2],
-                           [-1,+1,+1, +3,+2,+1],
                            [+1,+1,+1, -3,+2,+1],
-                           [+1,+1,-1, +3,-2,+1],
-                           [+1,-1,+1, +3,+2,-1]])],
+                           [-1,+1,+1, +1,-2, 3],
+                           [-1,+1,+1, +1,+3,-2],
+                           [-1,+1,+1, +2,-1,+3],
+                           [-1,+1,+1, +2,+3,-1],
+                           [-1,+1,+1, +3,+1,+2],
+                           [-1,+1,+1, +3,+2,+1]])],
                 'twin': [np.array([
-                           [-1, 1, 1,  2, 1, 1],
-                           [ 1, 1, 1, -2, 1, 1],
-                           [ 1, 1,-1,  2,-1, 1],
-                           [ 1,-1, 1,  2, 1,-1],
-                           [ 1,-1, 1,  1, 2, 1],
-                           [ 1, 1,-1, -1, 2, 1],
-                           [ 1, 1, 1,  1,-2, 1],
-                           [-1, 1, 1,  1, 2,-1],
-                           [ 1, 1,-1,  1, 1, 2],
-                           [ 1,-1, 1, -1, 1, 2],
-                           [-1, 1, 1,  1,-1, 2],
-                           [ 1, 1, 1,  1, 1,-2]])]
+                           [+1,-1,+1, +2,+1,-1],
+                           [+1,-1,+1, -1,+1,+2],
+                           [+1,-1,+1, +1,+2,+1],
+                           [-1,-1,+1, +2,-1,+1],
+                           [-1,-1,+1, +1,+1,+2],
+                           [-1,-1,+1, -1,+2,+1],
+                           [+1,+1,+1, +1,+1,-2],
+                           [+1,+1,+1, +1,-2,+1],
+                           [+1,+1,+1, -2,+1,+1],
+                           [-1,+1,+1, +1,-1,+2],
+                           [-1,+1,+1, +1,+2,-1],
+                           [-1,+1,+1, +2,+1,+1]])]
             },
             'hP': {
                 'slip': [np.array([
                            [+2,-1,-1, 0,  0, 0, 0,+1],
                            [-1,+2,-1, 0,  0, 0, 0,+1],
                            [-1,-1,+2, 0,  0, 0, 0,+1]]),
                          np.array([
@@ -1218,16 +1221,16 @@
         transform = [t for t in orientation_relationships[model].keys() if t.startswith(search)]    # type: ignore
 
         if len(transform) != 1:
             raise ValueError(f'invalid target lattice "{search.split(sep)[1]}"')
 
         m_l,o_l = transform[0].split(sep)                                                           # type: ignore
         m_p,o_p = orientation_relationships[model][m_l+sep+o_l]
-        other = Crystal(lattice=o_l) if target is None else target
-        m_p = np.stack((self.to_frame(uvw=m_p[:,0] if len(m_p[0,0])==3 else util.Bravais_to_Miller(uvtw=m_p[:,0])),
-                        self.to_frame(hkl=m_p[:,1] if len(m_p[0,1])==3 else util.Bravais_to_Miller(hkil=m_p[:,1]))),
-                        axis=1)
-        o_p = np.stack((other.to_frame(uvw=o_p[:,0] if len(o_p[0,0])==3 else util.Bravais_to_Miller(uvtw=o_p[:,0])),
-                        other.to_frame(hkl=o_p[:,1] if len(o_p[0,1])==3 else util.Bravais_to_Miller(hkil=o_p[:,1]))),
-                        axis=1)
-
+        m = Crystal(lattice=m_l) if self.parameters is None else Crystal(lattice=m_l,**self.parameters) # type: ignore
+        o = Crystal(lattice=o_l) if target is None else target
+        m_p = np.stack((m.to_frame(uvw=m_p[:,0] if len(m_p[0,0])==3 else util.Bravais_to_Miller(uvtw=m_p[:,0])),
+                        m.to_frame(hkl=m_p[:,1] if len(m_p[0,1])==3 else util.Bravais_to_Miller(hkil=m_p[:,1]))),
+                        axis=-2)
+        o_p = np.stack((o.to_frame(uvw=o_p[:,0] if len(o_p[0,0])==3 else util.Bravais_to_Miller(uvtw=o_p[:,0])),
+                        o.to_frame(hkl=o_p[:,1] if len(o_p[0,1])==3 else util.Bravais_to_Miller(hkil=o_p[:,1]))),
+                        axis=-2)
         return (o_l,Rotation.from_parallel(a=m_p,b=o_p))
```

### Comparing `damask-3.0.0b0/damask/_geomgrid.py` & `damask-3.0.0b2/damask/_geomgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             Valid extension is .vti, which will be appended if not given.
         label : str
             Label of the dataset containing the material IDs.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         """
         v = VTK.load(fname if str(fname).endswith('.vti') else str(fname)+'.vti')
         cells = np.array(v.vtk_data.GetDimensions())-1
         bbox  = np.array(v.vtk_data.GetBounds()).reshape(3,2).T
         ic = {l:v.get(l).reshape(cells,order='F') for l in set(v.labels['Cell Data']) - {label}}
 
@@ -251,15 +251,15 @@
         fname : str or pathlib.Path
             GeomGrid file to read.
             Valid extension is .vti, which will be appended if not given.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         """
         return GeomGrid._load(fname,'material')
 
 
     @staticmethod
     def load_SPPARKS(fname: Union[str, Path]) -> 'GeomGrid':
@@ -271,15 +271,15 @@
         fname : str or pathlib.Path
             SPPARKS VTK dump file to read.
             Valid extension is .vti, which will be appended if not given.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         Notes
         -----
         A SPPARKS VTI dump is equivalent to a DAMASK VTI file,
         but stores the materialID information as 'Spin' rather than 'material'.
 
         """
@@ -299,15 +299,15 @@
         ----------
         fname : str, pathlib.Path, or file handle
             Geometry file to read.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         """
         warnings.warn('Support for ASCII-based geom format will be removed in DAMASK 3.0.0', DeprecationWarning,2)
         if isinstance(fname, (str, Path)):
             f = open(fname)
         elif isinstance(fname, TextIO):
             f = fname
@@ -372,15 +372,15 @@
         ----------
         fname : str or pathlib.Path
             Geometry file to read.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         Notes
         -----
         Material indices in Neper usually start at 1 unless
         a buffer material with index 0 is added.
 
         Examples
@@ -447,23 +447,32 @@
             Path to the group (folder) that contains geometry (_SIMPL_GEOMETRY),
             and grain- or cell-wise data. Defaults to None, in which case
             it is set as the path that contains _SIMPL_GEOMETRY/SPACING.
 
         Returns
         -------
         loaded : damask.GeomGrid
-            GeomGrid-based geometry from file.
+            Grid-based geometry from file.
 
         Notes
         -----
-        damask.ConfigMaterial.load_DREAM3D gives the corresponding
-        material definition.
-
-        For cell-wise data, only unique combinations of
-        orientation and phase are considered.
+        A grain-wise geometry definition is based on segmented data from the
+        DREAM.3D file. This data is typically available when the microstructure
+        was synthetically created. In cell-wise representations, cells having
+        the same orientation and phase are grouped. Since synthetically created
+        microstructures have typically no in-grain scatter, cell-wise grids
+        can appear to be segmented.
+
+        damask.ConfigMaterial.load_DREAM3D creates the corresponding
+        material definition. Since the numbering of materials in cell-wise
+        and grain-wise grids is different, it is imperative to use the same
+        mode for both load_DREAM3D functions. That means, if the "feature_IDs"
+        argument is used for this function, the correct material configuration
+        is only obtained if the "grain_data" argument is used when calling
+        damask.ConfigMaterial.load_DREAM3D.
 
         """
         with h5py.File(fname, 'r') as f:
             b = util.DREAM3D_base_group(f) if base_group is None else base_group
             c = util.DREAM3D_cell_data_group(f) if cell_data is None else cell_data
 
             cells  = f['/'.join([b,'_SIMPL_GEOMETRY','DIMENSIONS'])][()]
@@ -503,15 +512,15 @@
         labels : (sequence of) str
             Label(s) of the columns containing the material definition.
             Each unique combination of values results in one material ID.
 
         Returns
         -------
         new : damask.GeomGrid
-            GeomGrid-based geometry from values in table.
+            Grid-based geometry from values in table.
 
         """
         cells,size,origin = grid_filters.cellsSizeOrigin_coordinates0_point(table.get(coordinates))
 
         labels_ = [labels] if isinstance(labels,str) else labels
         unique,unique_inverse = np.unique(np.hstack([table.get(l) for l in labels_]),return_inverse=True,axis=0)
 
@@ -558,15 +567,15 @@
             Defaults to None, in which case materials are consecutively numbered.
         periodic : bool, optional
             Assume grid to be periodic. Defaults to True.
 
         Returns
         -------
         new : damask.GeomGrid
-            GeomGrid-based geometry from tessellation.
+            Grid-based geometry from tessellation.
 
         """
         weights_p: FloatSequence
         if periodic:
             weights_p = np.tile(weights,27)                                                         # Laguerre weights (1,2,3,1,2,3,...,1,2,3)
             seeds_p = np.vstack((seeds  -np.array([size[0],0.,0.]),seeds,  seeds  +np.array([size[0],0.,0.])))
             seeds_p = np.vstack((seeds_p-np.array([0.,size[1],0.]),seeds_p,seeds_p+np.array([0.,size[1],0.])))
@@ -614,15 +623,15 @@
             Defaults to None, in which case materials are consecutively numbered.
         periodic : bool, optional
             Assume grid to be periodic. Defaults to True.
 
         Returns
         -------
         new : damask.GeomGrid
-            GeomGrid-based geometry from tessellation.
+            Grid-based geometry from tessellation.
 
         """
         coords = grid_filters.coordinates0_point(cells,size).reshape(-1,3)
         tree = spatial.cKDTree(seeds,boxsize=size) if periodic else \
                spatial.cKDTree(seeds)
         try:
             material_ = tree.query(coords, workers = int(os.environ.get('OMP_NUM_THREADS',4)))[1]
@@ -701,15 +710,15 @@
             Number of periods per unit cell. Defaults to 1.
         materials : sequence of int, len (2)
             Material IDs. Defaults to (0,1).
 
         Returns
         -------
         new : damask.GeomGrid
-            GeomGrid-based geometry from definition of minimal surface.
+            Grid-based geometry from definition of minimal surface.
 
         Notes
         -----
         The following triply-periodic minimal surfaces are implemented:
           - Schwarz P
           - Double Primitive
           - Schwarz D
```

### Comparing `damask-3.0.0b0/damask/_loadcasegrid.py` & `damask-3.0.0b2/damask/_loadcasegrid.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/_orientation.py` & `damask-3.0.0b2/damask/_orientation.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,15 +67,15 @@
        - cP : primitive
        - cI : body-centered
        - cF : face-centered
 
     and inherits the corresponding crystal family.
     Specifying a Bravais lattice, compared to just the crystal family,
     extends the functionality of Orientation objects to include operations such as
-    "Schmid", "related", or "to_pole" that require a lattice type and its parameters.
+    "Schmid", "related", or "to_frame" that require a lattice type and its parameters.
 
     Examples
     --------
     An array of 3 x 5 random orientations reduced to the fundamental zone of tetragonal symmetry:
 
     >>> import damask
     >>> o=damask.Orientation.from_random(shape=(3,5),family='tetragonal').reduced
@@ -363,15 +363,15 @@
             Lattice plane normal aligned with lab frame z-direction.
 
         Returns
         -------
         new : damask.Orientation
 
         """
-        o = cls(**kwargs)
+        o = cls(**kwargs,rotation=[1,0,0,0])
         x = o.to_frame(uvw=uvw)
         z = o.to_frame(hkl=hkl)
         om = np.stack([x,np.cross(z,x),z],axis=-2)
         return o.copy(Rotation.from_matrix(tensor.transpose(om/np.linalg.norm(om,axis=-1,keepdims=True))))
 
 
     @property
@@ -544,29 +544,31 @@
         s_o   = util.shapeshifter(other.shape,blend,mode='left')
 
         s =  self.broadcast_to(s_m).equivalent
         o = other.broadcast_to(s_o).equivalent
 
         r_ = s[:,np.newaxis,...].misorientation(o[np.newaxis,:,...]) # type: ignore[index]
         _r = ~r_
+        shp = r_.shape[2:]
 
         forward = r_.in_disorientation_FZ
         reverse = _r.in_disorientation_FZ
         ok  = forward | reverse
-        ok &= (np.cumsum(ok.reshape((-1,)+blend),axis=0) == 1).reshape(ok.shape)
+        ok &= (np.cumsum(ok.reshape((-1,*shp)),axis=0) == 1).reshape(ok.shape)
         r = np.where(np.any((ok&forward)[...,np.newaxis],axis=(0,1),keepdims=True),
                      r_.quaternion,
                      _r.quaternion)
         loc  = np.where(ok)
         sort = 0 if len(loc) == 2 else np.lexsort(loc[:1:-1])
-        quat = r[ok][sort].reshape(blend+(4,))
+
+        quat = r[ok][sort].reshape((*shp,4))
 
         return (
                 (self.copy(rotation=quat),
-                 (np.vstack(loc[:2]).T)[sort].reshape(blend+(2,)))
+                 (np.vstack(loc[:2]).T)[sort].reshape((*shp,2)))
                 if return_operators else
                 self.copy(rotation=quat)
                )
 
 
     def average(self,
                 weights: Optional[FloatSequence] = None,
@@ -615,15 +617,15 @@
                return_operators: bool = False) -> np.ndarray:
         """
         Rotate lab frame vector to ensure it falls into (improper or proper) standard stereographic triangle of crystal symmetry.
 
         Parameters
         ----------
         vector : numpy.ndarray, shape (...,3)
-            Lab frame vector to align with crystal frame direction.
+            Lab frame vector to align with an SST crystal frame direction.
             Shape of vector blends with shape of own rotation array.
             For example, a rotation array of shape (3,2) and a vector array of shape (2,4) result in (3,2,4) outputs.
         proper : bool, optional
             Consider only vectors with z >= 0, hence combine two neighboring SSTs.
             Defaults to False.
         return_operators : bool, optional
             Return the symmetrically equivalent orientation that rotated vector to SST.
@@ -637,16 +639,16 @@
             Index of symmetrically equivalent orientation that rotated vector to SST.
 
         """
         vector_ = np.array(vector,float)
         if vector_.shape[-1] != 3:
             raise ValueError('input is not a field of three-dimensional vectors')
 
-        blend = util.shapeblender( self.shape,vector_.shape[:-1])
-        eq    = self.broadcast_to(util.shapeshifter( self.shape,blend,mode='right')).equivalent
+        blend = util.shapeblender(self.shape,vector_.shape[:-1])
+        eq    = self.broadcast_to(util.shapeshifter(self.shape,blend,mode='right')).equivalent
         poles = np.atleast_2d(eq @ np.broadcast_to(vector_,(1,)+blend+(3,)))
         ok    = self.in_SST(poles,proper=proper)
         ok   &= np.cumsum(ok,axis=0) == 1
         loc   = np.where(ok)
         sort  = 0 if len(loc) == 1 else np.lexsort(loc[:0:-1])
 
         return (
@@ -783,19 +785,66 @@
 
         return rgb
 
 
 ####################################################################################################
     # functions that require lattice, not just family
 
-    def to_pole(self, *,
-                uvw: Optional[FloatSequence] = None,
-                hkl: Optional[FloatSequence] = None,
-                with_symmetry: bool = False,
-                normalize: bool = True) -> np.ndarray:
+    def to_lattice(self, *,
+                   direction: Optional[FloatSequence] = None,
+                   plane: Optional[FloatSequence] = None) -> np.ndarray:
+        """
+        Calculate lattice vector corresponding to lab frame direction or plane normal.
+
+        Parameters
+        ----------
+        direction|plane : numpy.ndarray, shape (...,3)
+            Real space vector along direction or
+            reciprocal space vector along plane normal.
+            Shape of vector blends with shape of own rotation array.
+            For example, a rotation array of shape (3,2) and a vector
+            array of shape (2,4) result in (3,2,4) outputs.
+
+        Returns
+        -------
+        Miller : numpy.ndarray, shape (...,3)
+            Lattice vector of direction or plane.
+            Use util.scale_to_coprime to convert to (integer) Miller indices.
+
+        Examples
+        --------
+        >>> import np
+        >>> import damask
+        >>> np.set_printoptions(precision=2,suppress=True,floatmode='maxprec')
+        >>> cubic = damask.Orientation.from_axis_angle(n_omega=[1,0,0,90],degrees=True,lattice='cI')
+        >>> cubic.to_lattice(direction=[1, 0, 0])
+        array([1., 0., 0.])
+        >>> cubic.to_lattice(direction=[0, 1, 0])
+        array([ 0.,  0., -1.])
+        >>> cubic.to_lattice(direction=[0, 0, 1])
+        array([-0.,  1.,  0.])
+        >>> tetragonal = damask.Orientation(lattice='tI',c=0.5)
+        >>> damask.util.scale_to_coprime(tetragonal.to_lattice(direction=[1,1,1]))
+        array([1, 1, 2])
+        >>> damask.util.scale_to_coprime(tetragonal.to_lattice(plane=[1,1,1]))
+        array([2, 2, 1])
+
+        """
+        if (direction is not None) ^ (plane is None):
+            raise KeyError('specify either "direction" or "plane"')
+        return (super().to_lattice(direction=self@np.asarray(direction)) if plane is None else
+                super().to_lattice(plane=self@np.asarray(plane)))
+
+
+    def to_frame(self, *,
+                 uvw: Optional[FloatSequence] = None,
+                 hkl: Optional[FloatSequence] = None,
+                 with_symmetry: bool = False,
+                 normalize: bool = True,
+                 ) -> np.ndarray:
         """
         Calculate lab frame vector along lattice direction [uvw] or plane normal (hkl).
 
         Parameters
         ----------
         uvw|hkl : numpy.ndarray, shape (...,3)
             Miller indices of crystallographic direction or plane normal.
@@ -807,31 +856,33 @@
             Defaults to False.
         normalize : bool, optional
             Normalize output vector.
             Defaults to True.
 
         Returns
         -------
-        vector : numpy.ndarray, shape (...,3) or (...,N,3)
-            Lab frame vector (or vectors if with_symmetry) along
+        vector : numpy.ndarray, shape (...,3) or (N,...,3)
+            Lab frame vector (or N vectors if with_symmetry) along
             [uvw] direction or (hkl) plane normal.
 
         """
-        v = self.to_frame(uvw=uvw,hkl=hkl)
+        v = super().to_frame(uvw=uvw,hkl=hkl)
         s_v = v.shape[:-1]
         blend = util.shapeblender(self.shape,s_v)
         if normalize:
             v /= np.linalg.norm(v,axis=-1,keepdims=len(s_v)>0)
         if with_symmetry:
             sym_ops = self.symmetry_operations
             s_v   += sym_ops.shape
             blend += sym_ops.shape
             v = sym_ops.broadcast_to(s_v) @ v[...,np.newaxis,:]
 
-        return ~(self.broadcast_to(blend)) @ np.broadcast_to(v,blend+(3,))
+        return np.moveaxis(~(self.broadcast_to(blend)) @ np.broadcast_to(v,blend+(3,)),
+                           -2 if with_symmetry else 0,
+                           0)
 
 
     def Schmid(self, *,
                N_slip: Optional[IntSequence] = None,
                N_twin: Optional[IntSequence] = None) -> np.ndarray:
         u"""
         Calculate Schmid matrix P = d ⨂ n in the lab frame for selected deformation systems.
@@ -867,16 +918,16 @@
 
         kinematics,active = (self.kinematics('slip'),N_slip) if N_twin is None else \
                             (self.kinematics('twin'),N_twin)
         if active == '*': active = [len(a) for a in kinematics['direction']]
 
         if not active:
             raise ValueError('Schmid matrix not defined')
-        d = self.to_frame(uvw=np.vstack([kinematics['direction'][i][:n] for i,n in enumerate(active)]))
-        p = self.to_frame(hkl=np.vstack([kinematics['plane'][i][:n] for i,n in enumerate(active)]))
+        d = super().to_frame(uvw=np.vstack([kinematics['direction'][i][:n] for i,n in enumerate(active)]))
+        p = super().to_frame(hkl=np.vstack([kinematics['plane'][i][:n] for i,n in enumerate(active)]))
         P = np.einsum('...i,...j',d/np.linalg.norm(d,axis=1,keepdims=True),
                                   p/np.linalg.norm(p,axis=1,keepdims=True))
 
         shape = P.shape[0:1]+self.shape+(3,3)
 
         return ~self.broadcast_to(shape[:-2]) \
                @ np.broadcast_to(P.reshape(util.shapeshifter(P.shape,shape)),shape)
@@ -921,15 +972,14 @@
         [[0.924 0.383 0.000 0.000]
          [0.924 0.000 0.383 0.000]
          [0.924 0.000 0.000 0.383]]
 
         """
         lattice,o = self.relation_operations(model,target)
         target = Crystal(lattice=lattice) if target is None else target
-
         return Orientation(rotation=o*Rotation(self.quaternion)[np.newaxis,...],  # type: ignore
                           lattice=lattice,
                           b = self.b if target.ratio['b'] is None else self.a*target.ratio['b'],
                           c = self.c if target.ratio['c'] is None else self.a*target.ratio['c'],
                           alpha = None if 'alpha' in target.immutable else self.alpha,
                           beta  = None if 'beta'  in target.immutable else self.beta,
                           gamma = None if 'gamma' in target.immutable else self.gamma,
```

### Comparing `damask-3.0.0b0/damask/_result.py` & `damask-3.0.0b2/damask/_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from collections import defaultdict
 from collections.abc import Iterable
 from typing import Optional, Union, Callable, Any, Sequence, Literal, Dict, List, Tuple
 
 import h5py
 import numpy as np
 from numpy import ma
+from scipy import interpolate
 
 import damask
 from . import VTK
 from . import Orientation
 from . import Rotation
 from . import grid_filters
 from . import mechanics
@@ -592,19 +593,19 @@
 
     @property
     def _incs(self):
         return [int(i.split(prefix_inc)[-1]) for i in self._increments]
 
     @property
     def increments(self):
-        return [int(i.split(prefix_inc)[-1]) for i in self._visible['increments']]
+        return [i for i in self._visible['increments']]
 
     @property
     def times(self):
-        return [self._times[i] for i in self.increments]
+        return [self._times[int(i.split(prefix_inc)[-1])] for i in self.increments]
 
     @property
     def phases(self):
         return self._visible['phases']
 
     @property
     def homogenizations(self):
@@ -1141,38 +1142,40 @@
         q : str, optional
             Name of the dataset containing the crystallographic orientation as quaternions.
             Defaults to 'O'.
         uvw|hkl : numpy.ndarray of shape (3)
             Miller indices of crystallographic direction or plane normal.
         with_symmetry : bool, optional
             Calculate all N symmetrically equivalent vectors.
-            Defaults to True.
+            Defaults to False.
         normalize : bool, optional
             Normalize output vector.
             Defaults to True.
 
         """
         def pole(q: DADF5Dataset,
                  uvw: FloatSequence, hkl: FloatSequence,
                  with_symmetry: bool,
                  normalize: bool) -> DADF5Dataset:
             c = q['meta']['c/a'] if 'c/a' in q['meta'] else 1.0
             brackets = ['[]','()','⟨⟩','{}'][(uvw is None)*1+with_symmetry*2]
             label = 'p^' + '{}{} {} {}{}'.format(brackets[0],
-                                                  *(uvw if uvw else hkl),
-                                                  brackets[-1],)
+                                                 *(uvw if uvw else hkl),
+                                                 brackets[-1],)
             ori = Orientation(q['data'],lattice=q['meta']['lattice'],a=1,c=c)
 
             return {
-                    'data': ori.to_pole(uvw=uvw,hkl=hkl,with_symmetry=with_symmetry,normalize=normalize),
+                    'data': np.moveaxis(ori.to_frame(uvw=uvw,hkl=hkl,
+                                                     with_symmetry=with_symmetry,
+                                                     normalize=normalize),0,-2 if with_symmetry else 0),
                     'label': label,
                     'meta' : {
                               'unit':        '1',
                               'description': f'{"normalized " if normalize else ""}lab frame vector along lattice ' \
-                                             + ('direction' if uvw is not None else 'plane') \
+                                             + ('plane' if uvw is None else 'direction') \
                                              + ('s' if with_symmetry else ''),
                               'creator':     'add_pole'
                               }
                     }
 
         self._add_generic_pointwise(pole,{'q':q},{'uvw':uvw,'hkl':hkl,'with_symmetry':with_symmetry,'normalize':normalize})
 
@@ -1933,18 +1936,17 @@
 
         at_cell_ph,in_data_ph,at_cell_ho,in_data_ho = self._mappings()
 
         out_dir = Path.cwd() if target_dir is None else Path(target_dir)
         out_dir.mkdir(parents=True,exist_ok=True)
 
         with h5py.File(self.fname,'r') as f:
-            if self.version_major == 1 or self.version_minor >= 13:
-                creator = f.attrs['creator'] if h5py3 else f.attrs['creator'].decode()
-                created = f.attrs['created'] if h5py3 else f.attrs['created'].decode()
-                v.comments += [f'{creator} ({created})']
+            creator = f.attrs['creator'] if h5py3 else f.attrs['creator'].decode()
+            created = f.attrs['created'] if h5py3 else f.attrs['created'].decode()
+            v.comments += [f'{creator} ({created})']
 
             for inc in util.show_progress(self._visible['increments']):
 
                 u = _read(f['/'.join([inc,'geometry','u_n' if mode.lower() == 'cell' else 'u_p'])])
                 v = v.set('u',u)
 
                 for ty in ['phase','homogenization']:
@@ -2121,19 +2123,24 @@
         ----------
         fname : str or pathlib.Path
             Name of the DADF5 file to be created.
         output : (list of) str, optional
             Names of the datasets to export.
             Defaults to '*', in which case all visible datasets are exported.
         mapping : numpy.ndarray of int, shape (:,:,:), optional
-            Indices for regridding.
+            Indices for regridding. Only applicable for grid
+            solver results.
 
         """
         if Path(fname).expanduser().absolute() == self.fname:
-            raise PermissionError(f'cannot overwrite {self.fname}')
+            raise PermissionError(f'cannot overwrite "{self.fname}"')
+
+        if mapping is not None and not self.structured:
+            raise PermissionError('cannot regrid unstructured mesh')
+
 
         def cp(path_in,path_out,label,mapping):
             if mapping is None:
                 path_in.copy(label,path_out)
             else:
                 path_out.create_dataset(label,data=path_in[label][()][mapping])
                 path_out[label].attrs.update(path_in[label].attrs)
@@ -2143,15 +2150,19 @@
             f_out.attrs.update(f_in.attrs)
             for g in ['setup','geometry'] + (['cell_to'] if mapping is None else []):
                 f_in.copy(g,f_out)
 
             if mapping is not None:
                 cells = mapping.shape
                 mapping_flat = mapping.flatten(order='F')
+
                 f_out['geometry'].attrs['cells'] = cells
+                if self.version_major == 1 and self.version_minor > 0:
+                    f_out['geometry']['cells'][...] = cells
+
                 f_out.create_group('cell_to')                                                       # ToDo: attribute missing
                 mappings = {'phase':{},'homogenization':{}}                                         # type: ignore
 
                 mapping_phase = f_in['cell_to']['phase'][()][mapping_flat]
                 for p in np.unique(mapping_phase['label']):
                     m = mapping_phase['label'] == p
                     mappings['phase'][p] = mapping_phase[m]['entry']
@@ -2172,16 +2183,21 @@
                 f_in.copy(inc,f_out,shallow=True)
                 if mapping is None:
                     for label in ['u_p','u_n']:
                         f_in[inc]['geometry'].copy(label,f_out[inc]['geometry'])
                 else:
                     u_p = f_in[inc]['geometry']['u_p'][()][mapping_flat]
                     f_out[inc]['geometry'].create_dataset('u_p',data=u_p)
-                    u_n = np.zeros((len(mapping_flat),3))                                           # ToDo: needs implementation
-                    f_out[inc]['geometry'].create_dataset('u_n',data=u_n)
+                    delta = self.size/np.array(mapping.shape)
+                    c_0_p = tuple([np.linspace(delta[i]/2,self.size[i]-delta[i]/2,mapping.shape[i]) for i in [0,1,2]])
+                    interpolator = interpolate.RegularGridInterpolator(c_0_p,np.reshape(u_p,tuple(cells)+(3,)),
+                                                                       fill_value=None,bounds_error=False,method='linear')
+                    c_0_n = grid_filters.coordinates0_node(mapping.shape,self.size).reshape(-1,3)
+                    f_out[inc]['geometry'].create_dataset('u_n',data=interpolator(c_0_n))
+                    f_out[inc]['geometry/u_n'].attrs.update(f_in[inc]['geometry/u_n'].attrs)
 
 
                 for label in self._homogenizations:
                     f_in[inc]['homogenization'].copy(label,f_out[inc]['homogenization'],shallow=True)
                 for label in self._phases:
                     f_in[inc]['phase'].copy(label,f_out[inc]['phase'],shallow=True)
```

### Comparing `damask-3.0.0b0/damask/_rotation.py` & `damask-3.0.0b2/damask/_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
         >>> r = damask.Rotation.from_random(shape=(12))
         >>> o = np.ones((12,3,3))
         >>> (r@o[np.newaxis,...]).shape                    # (12) @ (1,12, 3,3)
         (12,3,3,3)
 
         """
         if isinstance(other, np.ndarray):
-            obs = util.shapeblender(self.shape,other.shape)[len(self.shape):]
+            obs = (util.shapeblender(self.shape,other.shape[:-1])+other.shape[-1:])[len(self.shape):]
             for l in [4,2,1]:
                 if obs[-l:] == l*(3,):
                     bs = util.shapeblender(self.shape,other.shape[:-l],False)
                     self_ = self.broadcast_to(bs) if self.shape != bs else self
                     if l==1:
                         q_m = self_.quaternion[...,0]
                         p_m = self_.quaternion[...,1:]
@@ -626,22 +626,23 @@
         """
         Calculate misorientation to other Rotation.
 
         Parameters
         ----------
         other : damask.Rotation
             Rotation to which the misorientation is computed.
+            Compatible innermost dimensions will blend.
 
         Returns
         -------
         g : damask.Rotation
             Misorientation.
 
         """
-        return other/self
+        return ~(self*~other)
 
 
     ################################################################################################
     # convert to different orientation representations (numpy arrays)
 
     def as_quaternion(self) -> np.ndarray:
         """
@@ -959,17 +960,17 @@
         if reciprocal:
             om = np.linalg.inv(tensor.transpose(om)/np.pi)                                          # transform reciprocal basis set
             orthonormal = False                                                                     # contains stretch
 
         if not orthonormal:
             (U,S,Vh) = np.linalg.svd(om)                                                            # singular value decomposition
             om = np.einsum('...ij,...jl',U,Vh)
-        elif  not np.allclose(np.einsum('...i,...i',om[...,0],om[...,1]),0.) \
-           or not np.allclose(np.einsum('...i,...i',om[...,1],om[...,2]),0.) \
-           or not np.allclose(np.einsum('...i,...i',om[...,2],om[...,0]),0.):
+        elif  (np.abs(np.einsum('...i,...i',om[...,0],om[...,1])) > 5.e-8).any() \
+           or (np.abs(np.einsum('...i,...i',om[...,1],om[...,2])) > 5.e-8).any() \
+           or (np.abs(np.einsum('...i,...i',om[...,2],om[...,0])) > 5.e-8).any():
             raise ValueError('orientation matrix is not orthogonal')
 
         if not np.allclose(np.linalg.det(om),1.):
             raise ValueError('orientation matrix has determinant ≠ 1')
 
         return Rotation(Rotation._om2qu(om))
 
@@ -1011,15 +1012,15 @@
         Returns
         -------
         new : damask.Rotation
 
         """
         a_ = np.array(a,dtype=float)
         b_ = np.array(b,dtype=float)
-        if a_.shape[-2:] != (2,3) or b_.shape[-2:] != (2,3) or a_.shape != b_.shape:
+        if a_.shape[-2:] != (2,3) or b_.shape[-2:] != (2,3):
             raise ValueError('invalid shape')
         am = np.stack([          a_[...,0,:],
                                              a_[...,1,:],
                         np.cross(a_[...,0,:],a_[...,1,:]) ],axis=-2)
         bm = np.stack([          b_[...,0,:],
                                              b_[...,1,:],
                         np.cross(b_[...,0,:],b_[...,1,:]) ],axis=-2)
```

### Comparing `damask-3.0.0b0/damask/_table.py` & `damask-3.0.0b2/damask/_table.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/_typehints.py` & `damask-3.0.0b2/damask/_typehints.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/_vtk.py` & `damask-3.0.0b2/damask/_vtk.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/_yaml.py` & `damask-3.0.0b2/damask/_yaml.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def increase_indent(self,
                         flow: bool = False,
                         indentless: bool = False):
         return super().increase_indent(flow, False)                                                 # type: ignore
 
     def represent_data(self,
                        data: Any):
-        """Cast YAML objects and its subclasses to dict."""
+        """Cast YAML objects and their subclasses to dict."""
         if isinstance(data, dict) and type(data) != dict:
             return self.represent_data(dict(data))
         if isinstance(data, np.ndarray):
             return self.represent_data(data.tolist())
         if isinstance(data, Rotation):
             return self.represent_data(data.quaternion.tolist())
         if isinstance(data, np.generic):
@@ -77,21 +77,21 @@
         """
         New YAML-based configuration.
 
         Parameters
         ----------
         config : dict or str, optional
             YAML. String needs to be valid YAML.
-        **kwargs: arbitray keyword-value pairs, optional
-            Top level entries of the configuration.
+        **kwargs: arbitrary key–value pairs, optional
+            Top-level entries of the configuration.
 
         Notes
         -----
-        Values given as keyword-value pairs take precedence
-        over entries with the same keyword in 'config'.
+        Values given as key–value pairs take precedence
+        over entries with the same key in 'config'.
 
         """
         if int(platform.python_version_tuple()[1]) >= 9:
             if isinstance(config,str):
                 kwargs = yaml.load(config, Loader=SafeLoader) | kwargs
             elif isinstance(config,dict):
                 kwargs = config | kwargs                                                            # type: ignore
@@ -140,15 +140,15 @@
         Return self|other.
 
         Update configuration with contents of other.
 
         Parameters
         ----------
         other : damask.YAML or dict
-            Key-value pairs that update self.
+            Key–value pairs that update self.
 
         Returns
         -------
         updated : damask.YAML
             Updated configuration.
 
         Note
@@ -194,20 +194,20 @@
         return duplicate
 
 
     @classmethod
     def load(cls: Type[MyType],
              fname: FileHandle) -> MyType:
         """
-        Load from yaml file.
+        Load from YAML file.
 
         Parameters
         ----------
         fname : file, str, or pathlib.Path
-            Filename or file for writing.
+            Filename or file to read.
 
         Returns
         -------
         loaded : damask.YAML
             YAML from file.
 
         """
@@ -215,20 +215,20 @@
             return cls(yaml.load(fhandle, Loader=SafeLoader))
 
 
     def save(self,
              fname: FileHandle,
              **kwargs):
         """
-        Save to yaml file.
+        Save to YAML file.
 
         Parameters
         ----------
         fname : file, str, or pathlib.Path
-            Filename or file for writing.
+            Filename or file to write.
         **kwargs : dict
             Keyword arguments parsed to yaml.dump.
 
         """
         if 'width' not in kwargs:
             kwargs['width'] = 256
         if 'default_flow_style' not in kwargs:
```

### Comparing `damask-3.0.0b0/damask/grid_filters.py` & `damask-3.0.0b2/damask/grid_filters.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/mechanics.py` & `damask-3.0.0b2/damask/mechanics.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 Finite-strain continuum mechanics.
 
 All routines operate on numpy.ndarrays of shape (...,3,3).
 
 """
 
-from typing import Sequence as _Sequence#, Literal as _Literal
+from typing import Sequence as _Sequence, Union as _Union #, Literal as _Literal
 
 import numpy as _np
 
 from . import tensor as _tensor
 from . import _rotation
 
 
@@ -326,15 +326,15 @@
     where :math:`\vb{R}` is a rotation.
 
     """
     return _polar_decomposition(T,'U')[0]
 
 
 def _polar_decomposition(T: _np.ndarray,
-                         requested: _Sequence[str]) -> tuple:
+                         requested: _Union[str, _Sequence[str]]) -> tuple:
     """
     Perform singular value decomposition.
 
     Parameters
     ----------
     T : numpy.ndarray, shape (...,3,3)
         Tensor of which the singular values are computed.
@@ -345,15 +345,15 @@
     Returns
     -------
     VRU : tuple of numpy.ndarray, shape (...,3,3)
        Requested components of the singular value decomposition.
 
     """
     u, _, vh = _np.linalg.svd(T)
-    R = _np.einsum('...ij,...jk',u,vh)
+    R = u @ vh
 
     output = []
     if 'R' in requested:
         output+=[R]
     if 'V' in requested:
         output+=[_np.einsum('...ij,...kj',T,R)]
     if 'U' in requested:
```

### Comparing `damask-3.0.0b0/damask/seeds.py` & `damask-3.0.0b2/damask/seeds.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/solver/__init__.py` & `damask-3.0.0b2/damask/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/solver/_marc.py` & `damask-3.0.0b2/damask/solver/_marc.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/tensor.py` & `damask-3.0.0b2/damask/tensor.py`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/damask/util.py` & `damask-3.0.0b2/damask/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     Parameters
     ----------
     iterable : iterable
         Iterable to be decorated.
     N_iter : int, optional
         Total number of iterations. Required if iterable is not a sequence.
     prefix : str, optional
-        Prefix string.
+        Prefix string. Defaults to ''.
     bar_length : int, optional
         Length of progress bar in characters. Defaults to 50.
 
     """
     if isinstance(iterable,_abc.Sequence):
         if N_iter is None:
             N = len(iterable)
@@ -301,49 +301,53 @@
     else:
         status = ProgressBar(N,prefix,bar_length)
         for i,item in enumerate(iterable):
             yield item
             status.update(i)
 
 
-def scale_to_coprime(v: _FloatSequence) -> _np.ndarray:
+def scale_to_coprime(v: _FloatSequence,
+                     N_significant: int = 9) -> _np.ndarray:
     """
     Scale vector to co-prime (relatively prime) integers.
 
     Parameters
     ----------
     v : sequence of float, len (:)
         Vector to scale.
+    N_significant: int, optional
+        Number of significant digits to consider. Defaults to 9.
 
     Returns
     -------
     m : numpy.ndarray, shape (:)
         Vector scaled to co-prime numbers.
 
     """
-    MAX_DENOMINATOR = 1000000
 
-    def get_square_denominator(x):
+    def get_square_denominator(x,max_denominator):
         """Denominator of the square of a number."""
-        return _fractions.Fraction(x ** 2).limit_denominator(MAX_DENOMINATOR).denominator
+        return _fractions.Fraction(x ** 2).limit_denominator(max_denominator).denominator
 
     def lcm(a,b):
         """Least common multiple."""
         try:
-            return _np.lcm(a,b)                                                                      # numpy > 1.18
+            return _np.abs(_np.lcm(a,b))                                                            # numpy > 1.18
         except AttributeError:
-            return a * b // _np.gcd(a, b)
+            return _np.abs(a * b // _np.gcd(a, b))
 
-    v_ = _np.array(v)
-    m = (v_ * _reduce(lcm, map(lambda x: int(get_square_denominator(x)),v_))**0.5).astype(_np.int64)
+    max_denominator = int(10**(N_significant-1))
+
+    if (v_ := _np.asarray(v)).dtype in _np.sctypes['float']:
+        v_ = _np.round(_np.asarray(v,'float64')/_np.max(_np.abs(v)),N_significant)
+    m = (v_ * _reduce(lcm, map(lambda x: int(get_square_denominator(x,max_denominator)),v_))**0.5).astype(_np.int64)
     m = m//_reduce(_np.gcd,m)
 
-    with _np.errstate(invalid='ignore'):
-        if not _np.allclose(_np.ma.masked_invalid(v_/m),v_[_np.argmax(abs(v_))]/m[_np.argmax(abs(v_))]):
-            raise ValueError(f'invalid result "{m}" for input "{v_}"')
+    if not _np.allclose(m/_np.max(_np.abs(m)),v/_np.max(_np.abs(v)),atol=1e-2,rtol=0):
+        raise ValueError(f'invalid result "{m}" for input "{v}"')
 
     return m
 
 
 def project_equal_angle(vector: _np.ndarray,
                         direction: _Literal['x', 'y', 'z'] = 'z',                                   # noqa
                         normalize: bool = True,
```

### Comparing `damask-3.0.0b0/damask.egg-info/PKG-INFO` & `damask-3.0.0b2/damask.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damask
-Version: 3.0.0b0
+Version: 3.0.0b2
 Summary: DAMASK processing tools
 Home-page: https://damask.mpie.de
 Author: The DAMASK team
 Author-email: damask@mpie.de
 License: AGPL3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `damask-3.0.0b0/damask.egg-info/SOURCES.txt` & `damask-3.0.0b2/damask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `damask-3.0.0b0/setup.cfg` & `damask-3.0.0b2/setup.cfg`

 * *Files identical despite different names*

