# Comparing `tmp/comfit-1.4.2.tar.gz` & `tmp/comfit-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfit-1.4.2.tar", last modified: Mon Mar 18 21:07:59 2024, max compression
+gzip compressed data, was "comfit-1.5.0.tar", last modified: Thu May 30 12:10:21 2024, max compression
```

## Comparing `comfit-1.4.2.tar` & `comfit-1.5.0.tar`

### file list

```diff
@@ -1,37 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.391772 comfit-1.4.2/
--rw-rw-rw-   0        0        0     1091 2023-09-04 08:11:24.000000 comfit-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      119 2024-03-18 21:07:59.390773 comfit-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2024-02-28 10:13:02.000000 comfit-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.326423 comfit-1.4.2/comfit/
--rw-rw-rw-   0        0        0      589 2024-02-05 17:18:15.000000 comfit-1.4.2/comfit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.345543 comfit-1.4.2/comfit/core/
--rw-rw-rw-   0        0        0       37 2024-01-21 15:21:51.000000 comfit-1.4.2/comfit/core/__init__.py
--rw-rw-rw-   0        0        0    99909 2024-03-18 20:08:09.000000 comfit-1.4.2/comfit/core/base_system.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.359104 comfit-1.4.2/comfit/models/
--rw-rw-rw-   0        0        0      418 2023-12-12 23:33:08.000000 comfit-1.4.2/comfit/models/__init__.py
--rw-rw-rw-   0        0        0    28389 2024-03-03 08:10:46.000000 comfit-1.4.2/comfit/models/bose_einstein_condensate.py
--rw-rw-rw-   0        0        0    37416 2024-03-18 15:48:04.000000 comfit-1.4.2/comfit/models/nematic_liquid_crystal.py
--rw-rw-rw-   0        0        0    51410 2024-03-18 20:09:56.000000 comfit-1.4.2/comfit/models/phase_field_crystal.py
--rw-rw-rw-   0        0        0     6830 2024-03-13 20:08:28.000000 comfit-1.4.2/comfit/models/quantum_mechanics.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.377246 comfit-1.4.2/comfit/tools/
--rw-rw-rw-   0        0        0      372 2024-02-05 17:18:15.000000 comfit-1.4.2/comfit/tools/__init__.py
--rw-rw-rw-   0        0        0     2738 2024-03-13 20:08:28.000000 comfit-1.4.2/comfit/tools/tool_animation.py
--rw-rw-rw-   0        0        0     1185 2024-01-15 17:05:48.000000 comfit-1.4.2/comfit/tools/tool_colormaps.py
--rw-rw-rw-   0        0        0     1262 2024-01-21 10:23:03.000000 comfit-1.4.2/comfit/tools/tool_create_orthonormal_triad.py
--rw-rw-rw-   0        0        0      452 2024-03-13 20:08:28.000000 comfit-1.4.2/comfit/tools/tool_export_plot_functions.py
--rw-rw-rw-   0        0        0      831 2024-03-13 20:08:28.000000 comfit-1.4.2/comfit/tools/tool_math_functions.py
--rw-rw-rw-   0        0        0     1442 2023-12-04 18:33:48.000000 comfit-1.4.2/comfit/tools/tool_plot_manipulation_functions.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.339554 comfit-1.4.2/comfit.egg-info/
--rw-rw-rw-   0        0        0      119 2024-03-18 21:07:59.000000 comfit-1.4.2/comfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-03-18 21:07:59.000000 comfit-1.4.2/comfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 21:07:59.000000 comfit-1.4.2/comfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-18 21:07:59.000000 comfit-1.4.2/comfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-18 21:07:59.000000 comfit-1.4.2/comfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 21:07:59.391772 comfit-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-03-18 21:05:20.000000 comfit-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:07:59.388774 comfit-1.4.2/tests/
--rw-rw-rw-   0        0        0    27609 2024-03-06 20:12:55.000000 comfit-1.4.2/tests/test_base_system.py
--rw-rw-rw-   0        0        0     3462 2024-03-03 10:13:50.000000 comfit-1.4.2/tests/test_bose_einstein_condensate.py
--rw-rw-rw-   0        0        0     3237 2024-03-16 10:52:00.000000 comfit-1.4.2/tests/test_nematic_liquid_crystal.py
--rw-rw-rw-   0        0        0    18399 2024-03-03 09:57:51.000000 comfit-1.4.2/tests/test_phase_field_crystal.py
--rw-rw-rw-   0        0        0     1671 2024-03-04 08:08:21.000000 comfit-1.4.2/tests/test_quantum_mechanics.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.663323 comfit-1.5.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-08 21:02:57.000000 comfit-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      293 2024-05-30 12:10:21.661322 comfit-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3441 2024-05-02 07:52:44.000000 comfit-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.587284 comfit-1.5.0/comfit/
+-rw-rw-rw-   0        0        0      570 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.622305 comfit-1.5.0/comfit/core/
+-rw-rw-rw-   0        0        0       37 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/core/__init__.py
+-rw-rw-rw-   0        0        0      561 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/core/base_system.py
+-rw-rw-rw-   0        0        0    34794 2024-04-25 11:16:03.000000 comfit-1.5.0/comfit/core/base_system_calc.py
+-rw-rw-rw-   0        0        0      133 2024-04-25 11:16:26.000000 comfit-1.5.0/comfit/core/base_system_conf.py
+-rw-rw-rw-   0        0        0     3078 2024-04-25 11:17:48.000000 comfit-1.5.0/comfit/core/base_system_evolve.py
+-rw-rw-rw-   0        0        0     2790 2024-04-25 11:22:44.000000 comfit-1.5.0/comfit/core/base_system_get.py
+-rw-rw-rw-   0        0        0     7263 2024-05-30 11:28:29.000000 comfit-1.5.0/comfit/core/base_system_init.py
+-rw-rw-rw-   0        0        0    53489 2024-05-30 11:28:29.000000 comfit-1.5.0/comfit/core/base_system_plot.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.637511 comfit-1.5.0/comfit/models/
+-rw-rw-rw-   0        0        0      662 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/models/__init__.py
+-rw-rw-rw-   0        0        0    28790 2024-04-25 14:14:29.000000 comfit-1.5.0/comfit/models/bose_einstein_condensate.py
+-rw-rw-rw-   0        0        0    44229 2024-04-25 14:15:18.000000 comfit-1.5.0/comfit/models/nematic_liquid_crystal.py
+-rw-rw-rw-   0        0        0    33957 2024-05-30 11:28:29.000000 comfit-1.5.0/comfit/models/phase_field_crystal.py
+-rw-rw-rw-   0        0        0     3404 2024-04-25 14:29:30.000000 comfit-1.5.0/comfit/models/phase_field_crystal_1d_periodic.py
+-rw-rw-rw-   0        0        0     6338 2024-04-25 14:31:48.000000 comfit-1.5.0/comfit/models/phase_field_crystal_2d_square.py
+-rw-rw-rw-   0        0        0     5649 2024-04-25 14:33:33.000000 comfit-1.5.0/comfit/models/phase_field_crystal_2d_triangular.py
+-rw-rw-rw-   0        0        0     6449 2024-04-25 14:35:36.000000 comfit-1.5.0/comfit/models/phase_field_crystal_3d_body_centered_cubic.py
+-rw-rw-rw-   0        0        0     7543 2024-04-25 14:37:22.000000 comfit-1.5.0/comfit/models/phase_field_crystal_3d_face_centered_cubic.py
+-rw-rw-rw-   0        0        0     8489 2024-04-25 14:39:05.000000 comfit-1.5.0/comfit/models/phase_field_crystal_3d_simple_cubic.py
+-rw-rw-rw-   0        0        0     6542 2024-04-25 14:19:24.000000 comfit-1.5.0/comfit/models/quantum_mechanics.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.652929 comfit-1.5.0/comfit/tools/
+-rw-rw-rw-   0        0        0      372 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/tools/__init__.py
+-rw-rw-rw-   0        0        0     3809 2024-05-30 11:28:29.000000 comfit-1.5.0/comfit/tools/tool_animation.py
+-rw-rw-rw-   0        0        0     1185 2024-05-30 11:28:29.000000 comfit-1.5.0/comfit/tools/tool_colormaps.py
+-rw-rw-rw-   0        0        0     1262 2024-04-25 10:41:25.000000 comfit-1.5.0/comfit/tools/tool_create_orthonormal_triad.py
+-rw-rw-rw-   0        0        0      449 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/tools/tool_export_plot_functions.py
+-rw-rw-rw-   0        0        0      831 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/tools/tool_math_functions.py
+-rw-rw-rw-   0        0        0     1442 2024-04-08 21:02:57.000000 comfit-1.5.0/comfit/tools/tool_plot_manipulation_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.660316 comfit-1.5.0/comfit.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-05-30 12:10:21.000000 comfit-1.5.0/comfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1367 2024-05-30 12:10:21.000000 comfit-1.5.0/comfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:10:21.000000 comfit-1.5.0/comfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-30 12:10:21.000000 comfit-1.5.0/comfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:10:21.000000 comfit-1.5.0/comfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:10:21.663323 comfit-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      456 2024-05-30 12:07:12.000000 comfit-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:21.658426 comfit-1.5.0/tests/
+-rw-rw-rw-   0        0        0    27609 2024-04-08 21:02:59.000000 comfit-1.5.0/tests/test_base_system.py
+-rw-rw-rw-   0        0        0     3462 2024-04-08 21:02:59.000000 comfit-1.5.0/tests/test_bose_einstein_condensate.py
+-rw-rw-rw-   0        0        0     3347 2024-04-08 21:02:59.000000 comfit-1.5.0/tests/test_nematic_liquid_crystal.py
+-rw-rw-rw-   0        0        0    18399 2024-04-08 21:02:59.000000 comfit-1.5.0/tests/test_phase_field_crystal.py
+-rw-rw-rw-   0        0        0     1671 2024-04-08 21:02:59.000000 comfit-1.5.0/tests/test_quantum_mechanics.py
```

### Comparing `comfit-1.4.2/LICENSE` & `comfit-1.5.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `comfit-1.4.2/comfit/__init__.py` & `comfit-1.5.0/comfit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .core import BaseSystem
 
 from .models import BoseEinsteinCondensate, QuantumMechanics, \
-    PhaseFieldCrystal1DPeriodic, PhaseFieldCrystal, \
+    PhaseFieldCrystal1DPeriodic, \
     PhaseFieldCrystal2DTriangular, PhaseFieldCrystal2DSquare, \
     PhaseFieldCrystal3DBodyCenteredCubic, PhaseFieldCrystal3DFaceCenteredCubic, \
     PhaseFieldCrystal3DSimpleCubic, NematicLiquidCrystal
 
 from .tools import tool_colormap_bluewhitered, tool_colormap_angle, tool_save_plot, tool_make_animation_movie, tool_make_animation_gif, \
     tool_export_rotating_plot, tool_zoom_plot, tool_colormap_sunburst, tool_multinom
```

### Comparing `comfit-1.4.2/comfit/models/bose_einstein_condensate.py` & `comfit-1.5.0/comfit/models/bose_einstein_condensate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from comfit.core.base_system import BaseSystem
 from tqdm import tqdm
-from mpl_toolkits.mplot3d import Axes3D  # for 3D plotting
+from mpl_toolkits.mplot3d import Axes3D  
 import scipy as sp
 
-#A meaningless test comment
-
 class BoseEinsteinCondensate(BaseSystem):
     def __init__(self, dimension, **kwargs):
-        """
-        Initializes a system to simulate a Bose-Einstein Condensate using the Gross-Pitaevskii equation.
+        """Initializes a system to simulate a Bose-Einstein Condensate using the Gross-Pitaevskii equation.
+
+        Args:
+            dimension : int
+                The dimension of the system.
+            kwargs : dict, optional
+                Optional keyword arguments to set additional parameters. see
+                https://comfitlib.com/ClassBoseEinsteinCondensate/
 
-        Input:
-        - dimension : int
-            The dimension of the system.
-        - x_resolution : int
-            The resolution along the x-axis.
-        - kwargs : dict, optional
-            Optional keyword arguments to set additional parameters.
-
-        Output:
-        - BoseEinsteinCondensate object
-            The system object representing the BoseEinsteinCondensate simulation.
+        Returns:
+            The system object representing the BoseEinsteinCondensate simulation. BoseEinsteinCondensate object
 
         Example:
-        bec = BoseEinsteinCondensate(3, 100, dissipation_factor=0.5)
-        Creates a BoseEinsteinCondensate system with 3 dimensions and an x-resolution of 100. The dissipation factor is set to 0.5.
+            bec = BoseEinsteinCondensate(3,xRes=101,yRes=101,zRes=101, gamma=0.5)
+            Creates a BoseEinsteinCondensate system with 3 dimensions and a spatial resolution of 101 in all directions.
+            The dissipative factor gamma is set to 0.5.
         """
 
         # First initialize the BaseSystem class
         super().__init__(dimension, **kwargs)
 
         # Type of the system
         self.psi = None
         self.psi_f = None
         self.type = 'BoseEinsteinCondensate'
 
         # Default simulation parameters
-        self.gamma = 0.1 if 'gamma' not in kwargs else kwargs['gamma']  # Dissipation (gamma)
+        self.gamma = 0.01 if 'gamma' not in kwargs else kwargs['gamma']  # Dissipation (gamma)
 
         self.V_ext = lambda t: 0  # External potential, note this is a function of t
 
         # If there are additional arguments provided, set them as attributes
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def __str__(self):
-        """
-        Output a string representation of the system.
+        """Output a string representation of the system.
+
+        Args:
+            None
+
+        Returns:
+            A string representation of the system.
         """
         return f"ComFiT object: BoseEinsteinCondensate\n \
                 Dimension: {self.dim}\n"
 
     # CONFIGURATION FUNCTIONS
     def conf_initial_condition_disordered(self, noise_strength=0.01):
-        """
-        Sets disordered initial condition for the BoseEinsteinCondensate with some thermal flcutiations
+        """Sets disordered initial condition for the BoseEinsteinCondensate with some thermal flcutiations
         
-        Input:
+        Args:
             noise_strength: the strength of the noise
 
-        Output:
+        Returns:
             Sets the value of self.psi and self.psi_f
         """
 
         if self.dim == 1:
             self.psi = np.random.rand(self.xRes) - 0.5 + \
                        1j * np.random.rand(self.xRes) - 0.5j
 
@@ -79,20 +79,21 @@
         else:
             raise Exception("Code for this dimension has not yet been implemented.")
 
         self.psi = noise_strength * self.psi
         self.psi_f = sp.fft.fftn(self.psi)
 
     def conf_external_potential(self, V_ext, additive=False):
-        """
-        Sets the external potential of the system.
-        Input:
+        """Sets the external potential of the system.
+
+        Args:
             V_ext (function or float): the external potential
             additive (bool, optional): whether to add the new potential to the existing potential or not
-        Output:
+
+        Returns:
             Modifies the value of self.V_ext
         """
 
         if not callable(V_ext):
             original_V_ext = V_ext  # Preserve the original value of V_ext
             V_ext = lambda t: original_V_ext
         
@@ -100,40 +101,39 @@
             self.V_ext = lambda t: self.V_ext(t) + V_ext(t)
         else:
             self.V_ext = V_ext
 
 
 
     def conf_initial_condition_Thomas_Fermi(self):
-        """
-        Finds the Thomas_Fermi ground state.
+        """Finds the Thomas_Fermi ground state.
+
         Must be precided by an energy relaxation to find the true ground state
 
-        Input:
+        Args:
             None
         
-        Output: 
-            sets the value of self.psi and self.psi_f
+        Returns: 
+            Sets the value of self.psi and self.psi_f
         """
         V_0 = np.zeros(self.dims) + self.V_ext(self.time)
         self.psi = np.emath.sqrt(1 - V_0)
 
         self.psi[V_0 > 1] = 0
         self.psi_f = sp.fft.fftn(self.psi)
 
     # CONFIGURATION FUNCTIONS
     def conf_insert_vortex(self, charge=1, position=None):
-        """
-        Sets the initial condition for a vortex dipole
+        """Sets the initial condition for a vortex dipole
 
-        Input:
+        Args:
             charge (int): the charge of the vortex
             position (list): the position of the vortex
 
-        Output:
+        Returns:
             Modifies the value of self.psi and self.psi_f
         """
         if not (self.dim == 2):
             raise Exception("The dimension of the system must be 2 for a single point vortex.")
 
         if position is None:
             position = [self.xmid, self.ymid]
@@ -144,21 +144,20 @@
             # TODO: maybe this needs to be formulated in terms of model parameters (Vidar 16.11.23)
             #  Answer: Homogeneous ground-state is now replaced by the Thomas-Fermi ground-state (Jonas 21.11.23 )
 
         self.psi = self.psi * np.exp(1j * self.calc_angle_field_single_vortex(position, charge=charge))
         self.psi_f = sp.fft.fftn(self.psi)
 
     def conf_insert_vortex_dipole(self, dipole_vector=None, dipole_position=None):
-        """
-        Sets the initial condition for a vortex dipole configuration in a 2-dimensional system.
+        """Sets the initial condition for a vortex dipole configuration in a 2-dimensional system.
 
-        Input:
+        Args:
             None
 
-        Output:
+        Returns:
             Modifies the value of self.psi and self.psi_f
 
         Raises:
             Exception: If the dimension of the system is not 2.
         """
         if not (self.dim == 2):
             raise Exception("The dimension of the system must be 2 for a vortex dipole configuration.")
@@ -172,74 +171,75 @@
         if dipole_position is None:
             dipole_position = self.rmid
 
         self.psi = self.psi * np.exp(1j * self.calc_angle_field_vortex_dipole(dipole_vector, dipole_position))
         self.psi_f = sp.fft.fftn(self.psi)
 
     def conf_insert_vortex_ring(self, position=None, radius=None, normal_vector=[0, 0, 1]):
-        """
-        Sets the initial condition for a vortex ring configuration in a 3-dimensional system
+        """Sets the initial condition for a vortex ring configuration in a 3-dimensional system
         
-        Input:
-            position (list): the position of the vortex ring
-            radius (float): the radius of the vortex ring
-            normal_vector (list): the normal vector of the vortex ring
+        Args:
+            position: the position of the vortex ring (list)
+            radius: the radius of the vortex ring (float)
+            normal_vector: the normal vector of the vortex ring (list)
         
-        Output:
+        Returns:
             Modifies the value of self.psi and self.psi_f
         """
         if not (self.dim == 3):
             raise Exception("The dimension of the system must be 3 for a vortex ring configuration.")
 
         if position is None:
             position = self.rmid
 
         if radius is None:
             radius = self.xmax / 3
 
         theta = self.calc_angle_field_vortex_ring(position=position, radius=radius, normal_vector=normal_vector)
 
         if self.psi is None:
-            self.psi = 1
+            self.conf_initial_condition_Thomas_Fermi()
 
         self.psi = self.psi * np.exp(1j * theta)
         self.psi_f = sp.fft.fftn(self.psi)
 
     def conf_vortex_remover(self, nodes, Area):
-        '''
+        '''Removes vortices
+        
         Function that finds and removes vortices outside of the area defined by the corners
         (x1,y1), (x1,y2), (x2,y1), (x2,y2)
 
-        Input:
+        Args:
             nodes (list) a list containing the vortices
             Area  (array) list on the format (x1,x2,y1,y2)
 
-        Output:
+        Returns:
             Modifies the value of self.psi and self.psi_f
         '''
         for vortex in nodes:
             x_coord = vortex['position'][0]
             y_coord = vortex['position'][1]
             if not (Area[0] < x_coord and x_coord < Area[1] \
                     and Area[2] < y_coord and y_coord < Area[3]):
                 self.conf_insert_vortex(charge=-1 * vortex['charge'], position=[x_coord + self.dx, y_coord])
                 # self.conf_insert_vortex(charge=vortex['charge'], position=[7, 0])
 
     def conf_dissipative_frame(self, d=7, wx=50, wy=50, wz=50):
-        '''
+        '''Configures a dissipative frame around the computational domain
+
         This function sets self.gamma so that it has a low value in the bulk and a large value near the edges.
         This sets a dissipative frame around the computational domain
         
-        Input:
-            d (float): length of the interface between the low gamma and high gamma regions
-            wx (float): distance fom center to the frame in x-direction
-            wy (float):    -- " --                         y-direction
-            wz (float):     -- " --                         z-direction
+        Args:
+            d: length of the interface between the low gamma and high gamma regions (float)
+            wx: distance fom center to the frame in x-direction (float)
+            wy:    -- " --                         y-direction (float)
+            wz:     -- " --                         z-direction (float)
         
-        Output:
+        Returns:
             modify self.gamma
         '''
         if self.dim == 2:
             X, Y = np.meshgrid(self.x, self.y, indexing='ij')
             gammax = self.gamma + 1 / 2 * (2 + np.tanh((X - self.xmid - wx) / d) - np.tanh((X - self.xmid + wx) / d))
             gammay = self.gamma + 1 / 2 * (2 + np.tanh((Y - self.ymid - wy) / d) - np.tanh((Y - self.ymid + wy) / d))
             self.gamma = np.real(np.maximum(gammax, gammay))
@@ -251,44 +251,42 @@
             self.gamma = np.real(np.maximum(gammax, gammay, gammaz))
         else:
             raise Exception("This feature is not yet available for the given dimension.")
 
 
     # Time evolution
     def evolve_dGPE(self, number_of_steps, method='ETD2RK'):
-        '''
-        Evolver for the dGPE.
+        '''Evolver for the dGPE.
         
-        Input:
-            number_of_steps (int) the number of time steps that we are evolving the equation
-            method (string, optional) the integration method we want to use. ETD2RK is sett as default
+        Args:
+            number_of_steps: the number of time steps that we are evolving the equation  (int)
+            method: the integration method we want to use. ETD2RK is sett as default  (string, optional)
         
-        Output:
+        Returns:
             Updates the self.psi and self.psi_f
        '''
 
         k2 = self.calc_k2()
         omega_f = (1j + self.gamma) * (1 - 1 / 2 * k2)
 
         integrating_factors_f, solver = self.calc_integrating_factors_f_and_solver(omega_f, method)
 
         for n in tqdm(range(number_of_steps), desc='evolving the dGPE'):
             self.psi, self.psi_f = solver(integrating_factors_f,
                                           self.calc_nonlinear_evolution_function_f,
                                           self.psi, self.psi_f)
 
     def evolve_relax(self, number_of_steps, method='ETD2RK'):
-        '''
-        Evolver for the dGPE in imaginary time that relax the equation closer to the ground state
+        '''Evolver for the dGPE in imaginary time that relax the equation closer to the ground state
         
-        Input:
-            number_of_steps (int) the number of time steps that we are evolving the equation
-            method (string, optional) the integration method we want to use. ETD2RK is sett as default
+        Args:
+            number_of_steps: the number of time steps that we are evolving the equation (int)
+            method: the integration method we want to use. ETD2RK is sett as default (string)
         
-        Output:
+        Returns:
             Updates the self.psi and self.psi_f
         '''
         temp_t = self.time
         gamma0 = self.gamma
 
         self.gamma = 1 - 1j
 
@@ -301,26 +299,26 @@
 
         self.gamma = gamma0
         self.time = temp_t
         
         self.conf_external_potential(temp_V)
 
     def evolve_comoving_dGPE(self, number_of_steps, velx, method='ETD2RK'):
-        '''
-        Evolver for the dGPE in the comoving frame.
+        '''Evolver for the dGPE in the comoving frame.
+
         This evolver assume that the stirring is in the x-direction and that gamma is spatialy dependent
         
-        Input:
-            number_of_steps (int) the number of time steps that we are evolving the equation
-            velx (float) velocity in x direction
-            method (string, optional) the integration method we want to use. ETD2RK is sett as default
+        Args:
+            number_of_steps: the number of time steps that we are evolving the equation (int)
+            velx: velocity in x direction (float) 
+            method: the integration method we want to use. ETD2RK is sett as default (string)
         
-        Output:
+        Returns:
             Updates the fields self.psi and self.psi_f
-            '''
+        '''
         k2 = self.calc_k2()
 
         omega_f = (1j) * (1 - 1 / 2 * k2) + velx * self.dif[0]
 
         if method == 'ETD2RK':
             integrating_factors_f = self.calc_evolution_integrating_factors_ETD2RK(omega_f)
             solver = self.evolve_ETD2RK_loop
@@ -333,275 +331,266 @@
         for n in tqdm(range(number_of_steps), desc='evolving the dGPE in the comoving frame'):
             self.psi, self.psi_f = solver(integrating_factors_f, self.calc_nonlinear_evolution_term_comoving_f,
                                           self.psi, self.psi_f)
 
     # CALCULATION FUNCTIONS
 
     def calc_nonlinear_evolution_function_f(self, psi, t):
-        """
-        Calculates the non-linear evolution term of the dGPE
+        """Calculates the non-linear evolution term of the dGPE
         
-        Input:
-             psi (numpy.ndarray): the wavefunction at a given time.
+        Args:
+            psi: the wavefunction at a given time. (numpy.ndarray)
         
-        Output:
-            (numpy.ndarray): the non-linear evolution term
+        Returns:
+            The non-linear evolution term (numpy.ndarray)
         """
         
         psi2 = np.abs(psi) ** 2
         return sp.fft.fftn((1j + self.gamma) * (-self.V_ext(t) - psi2) * psi)
 
     def calc_nonlinear_evolution_term_comoving_f(self, psi, t):
-        """
-        Calculates the non-linear evolution term of the dGPE when gamma is not a constant.
+        """Calculates the non-linear evolution term of the dGPE when gamma is not a constant.
+
         Relevant for example in the comoving frame when we have a dissipative frame around the edge.
         
-        Input:
-            psi (numpy.ndarray): the wavefunction at a given time.
+        Args:
+            psi: the wavefunction at a given time. (numpy.ndarray)
         
-        Output:
-            (numpy.ndarray): the non-linear evolution term
+        Returns:
+            the non-linear evolution term (numpy.ndarray)
         """
         psi2 = np.abs(psi) ** 2
         term1 = sp.fft.fftn(-(1j + self.gamma) * (self.V_ext(t) + psi2) * psi)
         term2 = sp.fft.fftn(self.gamma * psi)
         term3 = 0.5 * sp.fft.fftn(self.gamma * sp.fft.ifftn(-self.calc_k2() * sp.fft.fftn(psi)))
         return (term1 + term2 + term3)
 
         # Functions for callculationg properties of the BoseEinsteinCondensate
 
     def calc_superfluid_current(self):
-        """
-        Function that calculates the superfluid current
+        """Calculates the superfluid current
 
-        Input:
+        Args:
             None
         
-        Output:
-            (numpy.ndarray) the superfluid current
+        Returns:
+            The superfluid current (numpy.ndarray) 
         """
         if self.dim == 2:
             J_s = np.zeros((self.dim,self.xRes,self.yRes))
         elif self.dim == 3:
             J_s = np.zeros((self.dim, self.xRes, self.yRes,self.zRes))
         else:
             raise(Exception('Calculation of the  superfluid current is not implemented in this dimension'))
         for i in range(self.dim):
             J_s[i] = np.imag( np.conj(self.psi) * sp.fft.ifftn(1j*self.k[i] *self.psi_f ))
         return J_s
 
     def calc_velocity(self):
-        """
-        Calculates the weighted velocity field
+        """Calculates the weighted velocity field
         
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.ndarray) the weighted velocity field
+        Returns:
+            The weighted velocity field (numpy.ndarray) 
         """
         if self.dim == 2:
             u = np.zeros((self.dim, self.xRes, self.yRes))
         elif self.dim == 3:
             u = np.zeros((self.dim, self.xRes, self.yRes, self.zRes))
         else:
             raise (Exception('Calculation of the weighted velocity is not implemented in this dimension'))
         theta = np.angle(self.psi)
         for i in range(self.dim):
             u[i] = np.imag(np.exp(-1j*theta)* sp.fft.ifftn(1j * self.k[i] * self.psi_f))
         return u
 
     def calc_kinetic_energy(self):
-        """
-        Calculates the kinetic energy.
+        """Calculates the kinetic energy.
 
-        Input:
+        Args:
             None
 
-        Output:
-            (float) the kinetic energy
+        Returns:
+            The kinetic energy (float) 
         """
         u = self.calc_velocity()
         u2 = np.sum(u[i]**2 for i in range(self.dim))
         return 0.5*self.calc_integrate_field(u2)
 
 
     def calc_hamiltonian_density(self):
-        """
-        Function that calculates the hamiltonian density
+        """Calculates the hamiltonian density
 
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.ndarray) the hamiltonian density
+        Returns:
+            The hamiltonian density (numpy.ndarray) 
         """
         k2 = self.calc_k2()
         interaction_term = 1/2*np.abs(self.psi)**4
         potential_term = (self.V_ext(self.time) - 1 )* np.abs(self.psi)**2
         laplacian_term = -1/2 *np.real( np.conj(self.psi) * sp.fft.ifftn(-k2*self.psi_f))
         return laplacian_term +potential_term + interaction_term
 
     def calc_hamiltonian(self):
-        """
-        Function that calculates the Hamiltonian
+        """Function that calculates the Hamiltonian
 
-        Input:
+        Args:
             None
 
-        Output:
-            (Float) the Hamiltonian
+        Returns:
+            The Hamiltonian
         """
         H = self.calc_hamiltonian_density()
         return self.calc_integrate_field(H)
 
     def calc_harmonic_potential(self, R_tf):
-        """
-        Set returns a harmonic trap with R_tf being the Thomas-Fermi radius
+        """Calculates a harmonic trap with R_tf being the Thomas-Fermi radius
         
-        Input:
-                R_tf (float): The Thomas-Fermi radius
+        Args:
+            R_tf (float): The Thomas-Fermi radius
         
-        Output:
-                A harmonic potential
+        Returns:
+            A harmonic potential
         """
         trapping_strength = 1 / (R_tf ** 2)
         if self.dim == 1:
             return trapping_strength * (self.x - self.xmid) ** 2
         if self.dim == 2:
             return trapping_strength * (((self.x - self.xmid) ** 2).reshape(self.xRes, 1)
                                         + ((self.y - self.ymid) ** 2).reshape(1, self.yRes))
         if self.dim == 3:
             return trapping_strength * (((self.x - self.xmid) ** 2).reshape(self.xRes, 1, 1)
                                         + ((self.y - self.ymid) ** 2).reshape(1, self.yRes, 1)
                                         + ((self.z - self.zmid) ** 2).reshape(1, 1, self.zRes))
 
     def calc_gaussian_stirring_potential(self, size, strength, position):
-        """
-        Function for calculate a gaussian potential
+        """Calculates a gaussian potential
         
-        Input:
+        Args:
             size (float) size of the stirrer
             strength (float) strength of the stirrer, i.e how large the potential is at the stirrers position
             position (array) the position of the stirrer
        
-        Output:
-            (numpy.ndarray) a gaussian potential
+        Retuns:
+            A gaussian potential (numpy.ndarray) 
         """
 
         if self.dim == 1:
             return strength * np.exp(-(self.x - position[0]) ** 2 / size ** 2)
 
         elif self.dim == 2:
             return strength * np.exp(-(((self.x - position[0]) ** 2).reshape(self.xRes, 1)
                                        + ((self.y - position[1]) ** 2).reshape(1, self.yRes)) / (size ** 2))
         elif self.dim == 3:
             return strength * np.exp(-(((self.x - position[0]) ** 2).reshape(self.xRes, 1, 1)
                                        + ((self.y - position[1]) ** 2).reshape(1, self.yRes, 1)
                                        + ((self.z - position[2]) ** 2).reshape(1, 1, self.zRes)) / (size ** 2))
 
     def calc_force_on_external_potential(self):
-        """ 
-        Calculates the average force acting on the external potential.
+        """Calculates the average force acting on the external potential.
         
-        Input:
+        Args:
             None
         
-        Output:
-            (numpy.ndarray) average force on the potential
+        Returns:
+            Average force on the potential (numpy.ndarray) 
         """
         Force =np.zeros(self.dim)
         potential_f = sp.fft.ifftn(self.V_ext(self.time))
         for i in range(self.dim):
             Force_density = np.real(np.abs(self.psi)**2 * sp.fft.ifftn(1j*self.k[i]* potential_f))
             Force[i] = self.calc_integrate_field(Force_density)
         return Force
         #TODO: It is not clear to me exactly what this function does (Vidar 04.12.23)
 
 
 
-## Functions for calculating vortex properties
+    ## Functions for calculating vortex properties
     def calc_vortex_density(self, psi=None):
-        """
-        Calculates the vortex density of the system.
+        """Calculates the vortex density of the system.
 
-        Input:
-            psi (numpy.ndarray): The wavefunction of the system.
+        Args:
+            psi: The wavefunction of the system. (numpy.ndarray)
         
-        Output:
-            numpy.ndarray: The vortex density of the system.
+        Returns:
+            The vortex density of the system. numpy.ndarray
         """
         if psi is None:
             psi = self.psi
 
         return self.calc_defect_density([np.real(psi), np.imag(psi)])
 
     def calc_vortex_density_singular(self):
-        """
-        Calculates the vortex density of the system using the singular method.
+        """Calculates the vortex density of the system using the singular method.
 
-        Input:
+        Args:
             None
         
-        Output:
-            numpy.ndarray: The vortex density of the system.
+        Returns:
+            The vortex density of the system. (numpy.ndarray)
         """
         # TODO: Insert the correct value of the equilibrium of psi, based on theory (Vidar 03.12.23)
         return self.calc_defect_density([np.real(self.psi), np.imag(self.psi)])
 
     def calc_vortex_velocity_field(self, dt_psi, psi=None):
-        """
-        Calculates the vortex velocity field of the system.
+        """Calculates the vortex velocity field of the system.
 
-        Input:
-            dt_psi (numpy.ndarray): The time derivative of the wavefunction of the system.
-            psi (numpy.ndarray): The wavefunction of the system.
+        Args:
+            dt_psi: The time derivative of the wavefunction of the system. (numpy.ndarray)
+            psi: The wavefunction of the system. (numpy.ndarray)
 
-        Output:
-            numpy.ndarray: The vortex velocity field of the system. 
+        Returns:
+            The vortex velocity field of the system. numpy.ndarray: 
         """
         if psi is None:
             psi = self.psi
 
         return self.calc_defect_velocity_field([np.real(psi), np.imag(psi)],
                                         [np.real(dt_psi), np.imag(dt_psi)])
 
     def calc_vortex_nodes(self, dt_psi=None):
         """
         Calculate the positions and charges of vortex nodes based on the defect density.
 
-        Input:
-            dt_psi (numpy.ndarray): The time derivative of the wavefunction of the system.    
+        Args:
+            dt_psi: The time derivative of the wavefunction of the system.     (numpy.ndarray)
     
-        Output:
-            list: A list of dictionaries representing the vortex nodes. Each dictionary contains the following keys:
+        Returns:
+            List of dictionaries representing the vortex nodes. Each dictionary contains the following keys:
                   - 'position_index': The position index of the vortex node in the defect density array.
                   - 'charge': The charge of the vortex node.
                   - 'position': The position of the vortex node as a list [x, y].
                   - 'velocity': The velocity of the vortex node as a list [vx, vy].
         """
 
         # Calculate defect density
         rho = self.calc_vortex_density(self.psi)
 
         if dt_psi is not None:
             velocity_field = self.calc_vortex_velocity_field(dt_psi, self.psi)
 
         if self.dim == 2:
-            vortex_nodes = self.calc_defect_nodes(np.abs(rho))
+            vortex_nodes = self.calc_defect_nodes(np.abs(rho), 
+                                                    charge_tolerance = 0.2,
+                                                    integration_radius = self.a0)
             for vortex in vortex_nodes:
                 vortex['charge'] = np.sign(rho[vortex['position_index']])
                 if dt_psi is not None:
                     vortex['velocity'] = [velocity_field[0][vortex['position_index']], 
                                         velocity_field[1][vortex['position_index']]]
                 else:
                     vortex['velocity'] = [float('nan'), float('nan')]
         elif self.dim == 3:
-            vortex_nodes = self.calc_defect_nodes(
-                np.sqrt(rho[0]**2 + rho[1]**2 + rho[2]**2)
+            vortex_nodes = self.calc_defect_nodes(np.sqrt(rho[0]**2 + rho[1]**2 + rho[2]**2), 
+                                                charge_tolerance = 2*self.a0,
+                                                integration_radius = 2*self.a0
                 )
             for vortex in vortex_nodes:
                 tangent_vector = np.array([rho[i][vortex['position_index']] for i in range(3)]),
                 vortex['tangent_vector'] = tangent_vector[0]/np.linalg.norm(tangent_vector)
                 
                 if dt_psi is not None:
                     vortex['velocity'] = [velocity_field[0][vortex['position_index']], 
@@ -610,29 +599,33 @@
                 else:
                     vortex['velocity'] = [float('nan'), float('nan'), float('nan')]
 
         return vortex_nodes
 
     # Plot functions
 
-    def plot_vortex_nodes(self, vortex_nodes, ax=None):
-        """
-        Plots the vortex nodes in the system.
+    def plot_vortex_nodes(self, vortex_nodes, **kwargs):
+        """Plots the vortex nodes in the system.
 
-        Input:
+        Args:
             vortex_nodes (list): A list of dictionaries representing the vortex nodes. Each dictionary contains the following keys:
                                  - 'position_index': The position index of the vortex node in the defect density array.
                                  - 'charge': The charge of the vortex node.
                                  - 'position': The position of the vortex node as a list [x, y].
                                  - 'velocity': The velocity of the vortex node as a list [vx, vy].
-            ax (matplotlib.axes.Axes): The axes on which to plot the vortex nodes. If None, a new figure and axes are created.
-        
-        Output:
-            matplotlib.axes.Axes: The axes on which the vortex nodes are plotted.
-        """
+            -**kwargs: Keyword arguments for the plot.
+                See https://comfitlib.com/ClassBaseSystem/
+                for a full list of keyword arguments.
+        
+        Returns:
+            The axes on which the vortex nodes are plotted. (matplotlib.axes.Axes: )
+        """
+        # Check if an axis object is provided
+        fig = kwargs.get('fig', plt.gcf())
+        ax = kwargs.get('ax', None)
         if self.dim == 2:
 
             if ax == None:
                 ax = plt.gcf().add_subplot(111)
 
             x_coords_pos = []
             y_coords_pos = []
```

### Comparing `comfit-1.4.2/comfit/models/nematic_liquid_crystal.py` & `comfit-1.5.0/comfit/models/nematic_liquid_crystal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import numpy
 import numpy as np
 from comfit.core.base_system import BaseSystem
 import scipy as sp
 from tqdm import tqdm
 import matplotlib.pyplot as plt
+from comfit.tools.tool_colormaps import tool_colormap_angle, tool_colormap_bluewhitered, tool_colormap_sunburst
+from comfit.tools.tool_create_orthonormal_triad import tool_create_orthonormal_triad
+
 from comfit.tools.tool_math_functions import levi_civita_symbol
 from mpl_toolkits.mplot3d import axes3d
 import matplotlib.cm as cm
 from matplotlib.colors import Normalize
 
 class NematicLiquidCrystal(BaseSystem):
 
     def __init__(self, dimension, **kwargs):
-        """
-        Initializes a system to simulate a (active) nematic liquid crystal
+        """Initializes a system to simulate a (active) nematic liquid crystal
 
-        Input:
-        - dimension : int
-            The dimension of the system. Note that only d=2 is implemented at the moment
-        - x_resolution : int
-            The resolution along the x-axis.
-        - kwargs : dict, optional
-            Optional keyword arguments to set additional parameters.
+        Args:
+            dimension : The dimension of the system.
+            kwargs : dict, optional
+            Optional keyword arguments to set additional parameters. See
+            https://comfitlib.com/ClassNematicLiquidCrystal/
 
-        Output:
-        - nematic object
+        Returns:
+        - NematicLiquidCrystal object
             The system object representing the nematic simulation.
 
         Example:
-        nematic = nematic(2, 100, alpha=-0.5)
-        Creates a nematic system with 2 dimensions and an x-resolution of 100. The activity alpha is set to -0.5.
+            nematic = NematicLiquidCrystal(2, xRes=100, yRes = 100, alpha=-0.5)
+            Creates a nematic liquid crystal with 2 dimensions and a spatial resolution of 100.
+            The activity alpha is set to -0.5.
         """
         super().__init__(dimension, **kwargs)
 
         # Type of the system
         self.Q = None
         self.Q_f = None
         self.u = None
@@ -52,30 +53,34 @@
         self.eta = 1 if 'eta' not in kwargs else kwargs['eta'] # viscosity
 
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def __str__(self):
-        """
-        Output a string representation of the system.
+        """Output a string representation of the system.
+
+        Input:
+            None
+
+        Returns:
+            A string representation of the system.
         """
         return "NematicLiquidCrystal"
 
     # Initial condition
     def conf_initial_condition_ordered(self, noise_strength=0.01):
-        """
-        Initialises the system with the nematogens pointing in the x-direction in 2D and in the z-direction in 3D
+        """Configures the system with the nematogens pointing in the x-direction in 2D and in the z-direction in 3D
         with some random noise in the angle.
         
-        Input:
-             noise_strength (float): A meshure for how much noise to put in the angle
+        Args:
+             noise_strength: A meshure for how much noise to put in the angle (float)
         
-        Output:
-            Initialises self.Q  and self.Q_f
+        Returns:
+            Initialises self.Q and self.Q_f
         
         Raises:
             Exception if the dimension is not 2 or 3
         """
         if self.dim == 2:
             S0 = np.sqrt(self.B)
             theta_rand = noise_strength*np.random.randn(self.xRes,self.yRes)
@@ -115,28 +120,27 @@
             self.k2_press = self.calc_k2()
             self.k2_press[0, 0, 0] = 1  # for calculating pressure and velocity
 
         else:
             raise Exception("This dimension is not included for the moment")
 
     def conf_insert_disclination_dipole(self, dipole_vector=None, dipole_position=None):
-        """
-        Sets the initial condition for a disclination dipole configuration in a 2-dimensional system.
+        """Sets the initial condition for a disclination dipole configuration in a 2-dimensional system.
 
-        Input:
+        Args:
             None
 
-        Output:
-            None
+        Returns:
+            Configures self.Q and self.Q_f with a disclination dipole configuration.
 
         Raises:
             Exception: If the dimension of the system is not 2.
         """
         if not (self.dim == 2):
-            raise Exception("The dimension of the system must be 2 for a vortex dipole configuration.")
+            raise Exception("The dimension of the system must be 2 for a disclination dipole configuration.")
 
         if self.Q is None:
             self.conf_initial_condition_ordered(noise_strength=0)
 
         if dipole_vector is None:
             dipole_vector = [self.xmax / 3, 0]
 
@@ -144,43 +148,44 @@
             dipole_position = self.rmid
 
         psi = (self.Q[0] + 1j*self.Q[1]) * np.exp(1j * self.calc_angle_field_vortex_dipole(dipole_vector, dipole_position))
         self.Q[0] = np.real(psi)
         self.Q[1] = np.imag(psi)
         self.Q_f = sp.fft.fft2(self.Q)
 
-    def conf_initial_disclination_line(self, position=None,angle=np.pi/2,sign = 1):
-        """
-        Sets the initial condition for a disclination line in a 3-dimensional system.
+    def conf_initial_disclination_lines(self, position=None):
+        """Sets the initial condition for a disclination line in a 3-dimensional system.
+
         The dislocation is parralell to the z-axis
 
-        Input:
+        Args:
             position (list): the position of the dislocation. Only the position in the xy plane is used
             angle (float): the angle between the director and the z axis.
             sign (float): +1 or -1. Charge of the dislocation in the xy-plain
 
-        Output:
+        Returns:
             Sets the value of self.Q and self.Q_f
         """
         if not (self.dim == 3):
             raise Exception("The dimension of the system must be 3 for a disclination line configuration.")
 
         if position is None:
-            position = self.rmid
-
-
-        theta = 1/2*np.arctan2((self.y-position[1]),(self.x-position[0]))
+            position1 = [self.xmid+self.xmax/3, self.ymid]
+            position2 = [self.xmid - self.xmax/3, self.ymid]
 
 
+        theta_1 = 1/2*np.arctan2((self.y-position1[1]),(self.x-position1[0]))
+        theta_2 = -1/2*np.arctan2((self.y-position2[1]),(self.x-position2[0]))
+        theta = theta_1 +theta_2
 
         S0 = 1/8* self.C/self.A + 1/2 * np.sqrt(self.C**2 /(16*self.A**2) + 3*self.B)
 
-        nx =  np.cos(np.sign(sign)*theta)*np.sin(angle)
-        ny = np.sin(np.sign(sign)*theta)*np.sin(angle)
-        nz = np.cos(angle)*np.ones_like(nx)
+        nx =  np.cos(theta)
+        ny = np.sin(theta)
+        nz = np.zeros_like(nx)
 
         self.Q = np.zeros((5, self.xRes, self.yRes, self.zRes))
         self.Q[0] = S0 * (nx * nx - 1 / 3)
         self.Q[1] = S0 * (nx * ny)
         self.Q[2] = S0 * (nx * nz)
         self.Q[3] = S0 * (ny * ny - 1 / 3)
         self.Q[4] = S0 * (ny * nz)
@@ -191,92 +196,86 @@
         self.k2_press = self.calc_k2()
         self.k2_press[0, 0, 0] = 1
 
 
 
 
     def conf_active_channel(self,width,d=7):
-        """
-        Set the activity to zero everywhere exept for inside a channel of width "width"
+        """Configures the activity to zero everywhere exept for inside a channel of width "width"
         
-        Input:
-            width (float): width of the channel
-            d (float, optional): width of interface
+        Args:
+            width: width of the channel (float)
+            d: width of interface (float, optional)
         
-        Output:
-            updates the activity to the channel configuration.
+        Returns:
+            Updates the activity to the channel configuration.
         """
         if self.dim ==2:
             X, Y = np.meshgrid(self.x, self.y, indexing='ij')
             alpha_0 = self.alpha
             self.alpha = alpha_0*(1- 1 / 2 * (2 + np.tanh((X - self.xmid - width/2) / d) - np.tanh((X - self.xmid + width/2) / d)))
         else:
             raise Exception("The active channel is only permitted in two dimensions")
 
-#### calculations related to the flow field
+    ## calculations related to the flow field
     def conf_u(self,Q):
-        #TODO: This function needs a more descriptive name (Vidar 03.01.24)
         '''
         Updates the velocity and its fourier transform given a nematic field Q.
         
-        Input:
+        Args:
             (numpy.narray) the Q tensor
         
-        Output:
+        Returns:
             (numpy.narray) velocity
         '''
         F_af = self.calc_active_force_f(Q)
         F_pf = self.calc_passive_force_f(Q)
         p_f = self.calc_pressure_f(F_af,F_pf)
         grad_pf = self.calc_grad_p_f(p_f)
         self.u_f = (F_af + F_pf-grad_pf )/ (self.Gamma +self.eta*self.k2_press)
 
         self.u = np.real(sp.fft.ifftn(self.u_f, axes=(range(-self.dim, 0))))
 
     def calc_active_force_f(self,Q):
-        '''
-        Function that calculates the activ force in Fourier space.
+        '''Function that calculates the activ force in Fourier space.
         
-        Input:
-            Q (numpy.narray) the order parameter that we use to find the force.
+        Args:
+            Q: the order parameter that we use to find the force.  (numpy.narray) 
         
-        Output:
-            (numpy.narray) the active force in Fourier space
+        Returns:
+            The active force in Fourier space (numpy.narray) 
         '''
         F_af = []
         for j in range(self.dim):
             F_af.append(np.sum(1j*self.k[i]*sp.fft.fftn(self.alpha *self.get_sym_tl(Q,j,i),axes=(range(-self.dim, 0)) ) for i in range(self.dim)))
         return np.array(F_af)
 
     def calc_passive_force_f(self,Q):
-        '''
-        Calculate the passive force in Fourier space
+        '''Calculates the passive force in Fourier space
         
-        Input:
-            Q (numpy.narray) the order parameter that we use to find the force.
+        Args:
+            Q: the order parameter that we use to find the force. (numpy.narray)
         
-        Output: 
-            numpy.ndarray: the passive force in Fourier space
+        Returns: 
+            The passive force in Fourier space numpy.ndarray: 
         '''
         Pi_f = self.calc_passive_stress_f(Q)
         F_pf = []
         for j in range(self.dim):
             F_pf.append(np.sum(1j * self.k[i] *Pi_f[j][i] for i in range(self.dim)))
         return numpy.array(F_pf)
 
     def calc_passive_stress_f(self,Q):
-        #TODO Make 3d
-        """
-        Calculates the passive stress in fourier space
+        """Calculates the passive stress in fourier space
 
-        Input:
-            Q (numpy.narray) the order parameter that we use to find the stress.
+        Args:
+            Q: the order parameter that we use to find the stress.
         
-        Output: 
-            (numpy.narray) the passive stress in fourier space
+        Returns: 
+            The passive stress in fourier space (numpy.narray) 
         """
         if self.dim == 2:
             H = self.calc_molecular_field(Q)
             Antisym_QH = np.sum(self.get_sym_tl(Q,0,k)*self.get_sym_tl(H,k,1) -self.get_sym_tl(H,0,k)*self.get_sym_tl(Q,k,1) for k in range(self.dim))
             Ericksen = np.zeros((self.dim,self.xRes,self.yRes),dtype=np.complex128)
             Ericksen[0] = - self.K*np.sum(sp.fft.ifftn(1j*self.k[0]*sp.fft.fftn(self.get_sym_tl(Q,m,l)))*
                                               sp.fft.ifftn(1j * self.k[0] * sp.fft.fftn(self.get_sym_tl(Q,m,l)))
@@ -333,22 +332,21 @@
         if self.dim == 2:
             return 2*( Q[0]**2 + Q[1]**2)
         elif self.dim == 3:
             return 2 *(Q[0]**2 + Q[1]**2+ Q[2]**2+Q[3]**2 + Q[4]**2 + Q[0]*Q[3])
 
 
     def calc_molecular_field(self,Q):
-        """
-        Finds the molecular field (NB! need to be rewriten when C != 0)
+        """Finds the molecular field 
         
-        Input:
+        Args:
             Q (numpy.ndarray): The nematic tensor
         
-        Output:
-             (numpy.ndarray): The molecular field
+        Returns:
+            The molecular field (numpy.ndarray)
         """
 
         Q2 =  self.calc_trace_Q2(Q)
         temp = -self.K * sp.fft.ifftn( self.k2* sp.fft.fftn(Q,axes=(range(-self.dim,0))),axes=(range(-self.dim,0)) )
 
         if self.dim == 2 or self.C == 0:
             return temp +self.A*self.B*Q -2*self.A*Q2*Q
@@ -362,53 +360,50 @@
             C_term[3] = self.C * (Q[1]**2 + Q[3]**2 +Q[4]**2 - 1/3 *Q2)
             C_term[4] = self.C * (Q[1]*Q[2]  -Q[4]*Q[0] )
 
             return temp +self.A*self.B*Q -2*self.A*Q2*Q +C_term
 
 
     def calc_pressure_f(self,F_af,F_pf):
-        '''
-        Calculates the pressure in Fourier space. The zero mode is set to zero
+        '''Calculates the pressure in Fourier space. The zero mode is set to zero
         
-        Input:
-            F_af (numpy.narray) the active force in Fourier space
-            F_pf (numpy.narray) the passive force in Fourier space
+        Args:
+            F_af: the active force in Fourier space  (numpy.narray)
+            F_pf:the passive force in Fourier space  (numpy.narray) 
         
-        Output:
-            (numpy.ndarray) the pressure
+        Returns: 
+            The pressure (numpy.ndarray) 
         '''
         p_af = np.sum(1j*self.k[i]*F_af[i] for i in range(self.dim))
         p_pf = np.sum(1j*self.k[i]*F_pf[i] for i in range(self.dim))
         return -(p_af + p_pf)/self.k2_press
 
-    #TODO: This function needs a more descriptive name (Vidar 21.01.24)
+    
     def calc_grad_p_f(self,p_f):
-        """
-        Caclulates the gradient of the pressure
+        """Caclulates the gradient of the pressure
         
-        Input: 
-            p_f (numpy.narray) the pressure in Fourier space
+        Args: 
+            p_f: the pressure in Fourier space  (numpy.narray)
         
-        Output:
-             (numpy.ndarray) gradient of th epressure
+        Returns:
+            Gradient of the pressure (numpy.ndarray) 
         """
         grad_pf = []
         for i in range(self.dim):
             grad_pf.append(1j*self.k[i]*p_f)
         return np.array(grad_pf)
 
     def calc_vorticity_tensor(self):
-        """
-        Calculates the vorticity tensor
+        """Calculates the vorticity tensor
 
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.ndarray) The vorticity tensor
+        Returns:
+            The vorticity tensor (numpy.ndarray) 
         """
         if self.dim == 2:
 
             Omega_f = (1j*self.k[0]*self.u_f[1] -1j*self.k[1]*self.u_f[0])/2
             Omega = sp.fft.ifftn(Omega_f,axes=range(-self.dim,0))
             return np.real(Omega)
 
@@ -418,42 +413,39 @@
             Omega[1] = np.real(sp.fft.ifftn((1j * self.k[0] * self.u_f[2] - 1j * self.k[2] * self.u_f[0]) / 2,
                                             axes=range(-self.dim, 0)))
             Omega[2] = np.real(sp.fft.ifftn((1j * self.k[1] * self.u_f[2] - 1j * self.k[2] * self.u_f[1]) / 2,
                                             axes=range(-self.dim, 0)))
             return Omega
 
     def calc_strain_rate_tensor_f(self):
-        # TODO Make symetric and 3d
         """
         Calculates the strainrate tensor
 
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.ndarray) The strainrate
+        Returns: 
+            The strainrate (numpy.ndarray) 
         """
         E_f = np.zeros_like(self.Q_f)
         for i in range(self.dim):
             for j in range(self.dim):
                 E_f[i][j]= (1j*self.k[i]*self.u_f[j] +1j*self.k[j]*self.u_f[i])/2
         return E_f
 
-#### Calculation of non-linear evolution terms
+    ## Calculation of non-linear evolution terms
     def calc_nonlinear_evolution_function_f(self,Q,t):
-        # TODO test and make sure that the passive stress works as intended (Jonas: 2023/11/14)
-        #TODO make 3d compatible
-        """
-        Calculates the non-linear evolution function for the nematic
+        """Calculates the non-linear evolution function for the nematic
         
-        Input:
-            Q (numpy.narray) the nematic orderparameter
+        Args:
+            Q: the nematic orderparameter (numpy.narray) 
         
-        Output:
-            (numpy.narray) the non-linear evolution function evaluated in Fourier space
+        Returns:
+            
+            The non-linear evolution function evaluated in Fourier space (numpy.narray) 
         """
         if self.dim == 2:
             self.conf_u(Q)
             Q_f = sp.fft.fftn(Q,axes=range(-self.dim,0))
             N_f = self.calc_nonlinear_evolution_term_no_flow_f(Q,t)
             Omega =self.calc_vorticity_tensor()
             Antisym_Omega_Q = np.zeros_like(Q_f)
@@ -462,15 +454,14 @@
             Antisym_Omega_Q[1] = 2*Q[0]*Omega
 
             advectiv_deriv = - np.sum(self.u[k]* sp.fft.ifftn(1j*self.k[k] * Q_f,axes=(range(-self.dim,0)))for k in range(self.dim) )
 
             return sp.fft.fftn(Antisym_Omega_Q +advectiv_deriv, axes=range(-self.dim,0)) +N_f
 
         elif self.dim == 3:
-            # TODO: check that antisym_omega is correct (18/01/24)
             self.conf_u(Q)
             Q_f = sp.fft.fftn(Q, axes=range(-self.dim, 0))
             N_f = self.calc_nonlinear_evolution_term_no_flow_f(Q,t)
             Omega = self.calc_vorticity_tensor()
 
             advectiv_deriv = - np.sum(
                 self.u[k] * sp.fft.ifftn(1j * self.k[k] * Q_f, axes=(range(-self.dim, 0))) for k in range(self.dim))
@@ -485,23 +476,21 @@
 
             return sp.fft.fftn(Antisym_Omega_Q + advectiv_deriv, axes=range(-self.dim, 0)) + N_f
 
         else:
             raise Exception("This dimension is not implemented at the moment")
 
     def calc_nonlinear_evolution_term_no_flow_f(self,Q,t):
-
-        """
-        Calculates the non-linear evolution function for the nematic without the flow field
+        """Calculates the non-linear evolution function for the nematic without the flow field
         
-        Input:
-            Q (numpy.narray) the nematic orderparameter
+        Args:
+            Q: the nematic orderparameter  (numpy.narray)
         
-        Output:
-            (numpy.narray) the non-linear evolution function evaluated in Fourier space
+        Returns:
+            The non-linear evolution function evaluated in Fourier space (numpy.narray) 
         """
         Q2 = self.calc_trace_Q2(Q)
         if self.dim ==2 or self.C == 0:
             return -2*self.A*sp.fft.fftn(Q2 *Q,axes =(range(-self.dim,0)))/self.gamma
 
         elif self.dim == 3:
             C_term = np.zeros((5, self.xRes, self.yRes, self.zRes))
@@ -512,22 +501,21 @@
             C_term[3] = self.C * (Q[1] ** 2 + Q[3] ** 2 + Q[4] ** 2 - 1 / 3 * Q2)
             C_term[4] = self.C * (Q[1] * Q[2] - Q[4] * Q[0])
             return -2*self.A*sp.fft.fftn(Q2 *Q,axes =(range(-self.dim,0)))/self.gamma + sp.fft.fftn(C_term ,axes =(range(-self.dim,0)))/self.gamma
 
 
 ##### evolvers
     def evolve_nematic(self, number_of_steps, method= 'ETD2RK'):
-        '''
-         Evolver for the nematic system
+        '''Evolves the nematic system
         
-        Input:
-            number_of_steps (int) the number of time steps that we are evolving the equation
-            method (string, optional) the integration method we want to use. ETD2RK is sett as default
+        Args:
+            number_of_steps: the number of time steps that we are evolving the equation  (int)
+            method: the integration method we want to use. ETD2RK is sett as default  (string)
         
-        Output:
+        Returns:
             Updates the fields self.Q and self.Q_f
         '''
         omega_f = (self.A * self.B - self.K * self.k2) / self.gamma
 
         if method == 'ETD2RK':
             integrating_factors_f = self.calc_evolution_integrating_factors_ETD2RK(omega_f)
             solver = self.evolve_ETD2RK_loop
@@ -541,21 +529,21 @@
             self.Q, self.Q_f = solver(integrating_factors_f,
                                                        self.calc_nonlinear_evolution_function_f,
                                                        self.Q, self.Q_f)
         self.Q = np.real(self.Q)
         self.conf_u(self.Q)
 
     def evolve_nematic_no_flow(self,number_of_steps,method = 'ETD2RK'):
-        ''' Evolver for the nematic system without the flow field
+        ''' Evolves the nematic system without the flow field
         
-        Input:
-            number_of_steps (int) the number of time steps that we are evolving the equation
-            method (string, optional) the integration method we want to use. ETD2RK is sett as default
+        Args:
+            number_of_steps: the number of time steps that we are evolving the equation  (int)
+            method: the integration method we want to use. ETD2RK is sett as default  (string)
         
-        Output:
+        Returns:
             Updates the fields self.Q and self.Q_f
         '''
         omega_f = (self.A * self.B - self.K * self.k2) / self.gamma
 
         if method == 'ETD2RK':
             integrating_factors_f = self.calc_evolution_integrating_factors_ETD2RK(omega_f)
             solver = self.evolve_ETD2RK_loop
@@ -568,108 +556,124 @@
 
         for n in tqdm(range(number_of_steps), desc='evolving the active nematic'):
             self.Q, self.Q_f = solver(integrating_factors_f,self.calc_nonlinear_evolution_term_no_flow_f,
                                                            self.Q, self.Q_f)
         self.Q = np.real(self.Q)
 
 
-##### defect tracking
+    ## Disclination tracking
     def calc_disclination_density_nematic(self):
-        #TODO: Optimize
         """
-        Calculates the defect density for the nematic. Note that in three dimension the defect density is a tensor
+        Calculates the disclination density for the nematic. Note that in three dimension the disclination density is a tensor
 
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.narray) The defect density
+        Returns:
+            The disclination density (numpy.narray) 
         """
         if self.dim == 2:
             psi0 = np.sqrt(self.B)/2
             psi =[self.Q[0],self.Q[1]]
             return self.calc_defect_density(psi, psi0)
 
         elif self.dim == 3:
             D = np.zeros((self.dim,self.dim,self.xRes,self.yRes,self.zRes))
-
-            term_trace = np.sum(sp.fft.ifftn(self.dif[k] * self.get_sym_tl(self.Q_f,k,a)) *
-                                       sp.fft.ifftn(self.dif[l]*self.get_sym_tl(self.Q_f,l,a))
-                                       for k in range(self.dim) for a in range(self.dim) for l in range(self.dim) )
-            term_trace -= np.sum(sp.fft.ifftn(self.dif[k] * self.get_sym_tl(self.Q_f,l,a)) *
-                                       sp.fft.ifftn(self.dif[l]*self.get_sym_tl(self.Q_f,k,a))
-                                       for k in range(self.dim) for a in range(self.dim) for l in range(self.dim) )
-            for i in range(self.dim):
-                for j in range(self.dim):
-                    term1 = 2 * np.sum(sp.fft.ifftn(self.dif[i] * self.get_sym_tl(self.Q_f,k,a)) *
-                                       sp.fft.ifftn(self.dif[k]*self.get_sym_tl(self.Q_f,j,a))
-                                       for k in range(self.dim) for a in range(self.dim))
-                    term2 = -2 * np.sum(sp.fft.ifftn(self.dif[i]*self.get_sym_tl(self.Q_f,j,a)) *
-                                        sp.fft.ifftn(self.dif[k] *self.get_sym_tl(self.Q_f,k,a))
-                                        for k in range(self.dim) for a in range(self.dim))
-                    D[i,j] = np.real(term1 + term2)
-                    if i == j:
-                        D[i,j] += np.real(term_trace)
+            term_trace = np.sum(np.real(sp.fft.ifftn(1j*self.k[k]* self.get_sym_tl(self.Q_f,k,a)))*
+                                    np.real(sp.fft.ifftn(1j*self.k[l] * self.get_sym_tl(self.Q_f,l,a)))
+                                    - np.real(sp.fft.ifftn(1j*self.k[k]* self.get_sym_tl(self.Q_f,l,a)))*
+                                    np.real(sp.fft.ifftn(1j*self.k[l] * self.get_sym_tl(self.Q_f,k,a)))
+                                    for k in range(self.dim) for a in range(self.dim) for l in range(self.dim))
+
+            for gam in range(self.dim):
+                for i in range(self.dim):
+                    D[gam, i] = 2*np.sum(np.real(sp.fft.ifftn(1j*self.k[gam]* self.get_sym_tl(self.Q_f,k,a)))*
+                                    np.real(sp.fft.ifftn(1j*self.k[k] * self.get_sym_tl(self.Q_f,i,a)))
+                                    - np.real(sp.fft.ifftn(1j*self.k[gam]* self.get_sym_tl(self.Q_f,i,a)))*
+                                    np.real(sp.fft.ifftn(1j*self.k[k] * self.get_sym_tl(self.Q_f,k,a)))
+                                    for k in range(self.dim) for a in range(self.dim))
+                    if gam == i:
+                        D[gam,i] += term_trace
             return D
         else:
-            raise Exception("Not implemented")
+            raise Exception("Only two and three dimensions are currently supported")
 
 
     def calc_disclination_density_decoupled(self):
+        """Calculates the decoupled diclination density
+
+        Args:
+            None
+        
+        Returns:
+            The disclination density (numpy.narray)
+        """ 
         if self.dim == 3:
             D = self.calc_disclination_density_nematic()
-            omega = np.sqrt(np.sum(D[i,j]*D[i,j] for i in range(self.dim) for j in range(self.dim)) )
+            S0 = self.calc_equilibrium_S()
+            rho = D/(S0**2 *np.pi)
+            omega = np.sqrt(np.sum(rho[i,j]*rho[i,j] for i in range(self.dim) for j in range(self.dim)) )
 
             DDT = np.zeros((self.xRes,self.yRes,self.zRes,self.dim,self.dim))
             DTD = np.zeros((self.xRes,self.yRes,self.zRes,self.dim,self.dim))
 
             for i in range(self.dim):
                 for j in range(self.dim):
-                    DDT[:,:,:,i,j] = np.sum(D[i,k]*D[j,k] for k in range(self.dim))
-                    DTD[:, :, :, i, j] = np.sum(D[k,i] * D[ k,j] for k in range(self.dim))
+                    DDT[:,:,:,i,j] = np.sum(rho[i,k]*rho[j,k] for k in range(self.dim))
+                    DTD[:, :, :, i, j] = np.sum(rho[k,i] * rho[ k,j] for k in range(self.dim))
 
-            vals_1,vecs_1 =  numpy.linalg.eig(DDT)
-            vals_2, vecs_2 = numpy.linalg.eig(DTD)
-            Omega = np.transpose(vecs_1[:,:,:,:,0], (3,0,1,2))
-            T = np.transpose(vecs_2[:,:,:,:,0], (3,0,1,2))
+            vals_1,vecs_1 =  numpy.linalg.eigh(DDT)
+            vals_2, vecs_2 = numpy.linalg.eigh(DTD)
+
+            Omega = np.transpose(vecs_1[:,:,:,:,2], (3,0,1,2))
+            T = np.transpose(vecs_2[:,:,:,:,2], (3,0,1,2))
             trD = np.sum(D[i,i] for i in range(self.dim))
             return omega, Omega, T, trD
 
 
     def calc_dt_psi(self,Q_prev,delta_t):
+        """Calculates the time derivative of the order parameter
+
+        Args:
+            Q_prev: the order parameter at the previous time step (numpy.narray)
+            delta_t: the time step (float)
+        
+        Returns:
+            The time derivative of the order parameter (numpy.narray)
+        """
+
         dt_Q = (self.Q -Q_prev)/delta_t
         return dt_Q[0] + 1j*dt_Q[1]
 
-    def calc_S(self):
-        # TODO: This function will be removed soon
-        '''
-        Calculates the strength of nematic order S
+    def calc_equilibrium_S(self):
+        '''Calculates the strength of nematic order S
 
-        Input:
+        Args:
             None
 
-        Output:
-            (numpy.narray) S
+        Returns:
+            equilibriums value of D (numpy.narray) 
         '''
         if self.dim == 2:
-            return 2 * np.sqrt((self.Q[0]) ** 2 + (self.Q[1]) ** 2)
+            return  np.sqrt(self.B)
 
         elif self.dim == 3:
-            Q2 = self.calc_trace_Q2(self.Q)
-            return np.sqrt(3 * Q2 / 2)
+            S0 = 1 / 8 * self.C / self.A + 1 / 2 * np.sqrt(self.C ** 2 / (16 * self.A ** 2) + 3 * self.B)
+            return S0
 
     def calc_order_and_director(self):
-        """
-        Finds the amount of order (S) and the director field (n)
+        """Calculates the amount of order (S) and the director field (n)
 
-        Input:
+        Args:
             None
 
-        Output:
-            (tuple): (scalar field) S - amount of order   , (vector field) the director field
+        Returns:
+            Tuple consisting of 
+                - Amount of order (scalar field) 
+                - the director field (vector field)
         """
         if self.dim == 2:
             psi_n = self.Q[0] + 1j*self.Q[1]
             angle = np.angle(psi_n)
             S =2 * np.sqrt((self.Q[0]) ** 2 + (self.Q[1]) ** 2)
             return S, [np.cos(angle/2),np.sin(angle/2)]
         elif self.dim ==3:
@@ -681,109 +685,145 @@
 
             eigvals, eigvectors = numpy.linalg.eigh(Q_eig)
             S = 3/2 *eigvals[:,:,:,2]
             n = np.transpose(eigvectors[:,:,:,:,2], (3,0,1,2))
 
             return S, n
 
-    def calc_vortex_velocity_field(self, dt_Q, psi=None):
+    def calc_disclination_velocity_field(self, dt_Q):
         """
-        Calculates the velocity field of the defect in two dimensions
-        
-        Input:
-            dt_Q (numpy.narray) the time derivative of the order parameter
-            psi (numpy.narray, optional) the order parameter
+        Calculates the velocity field of the disclination in two dimensions
         
-        Output:
-            (numpy.narray) the velocity field
+        Args:
+            dt_Q: the time derivative of the order parameter (numpy.narray)
+
+        Returns:
+            The velocity field (numpy.narray) 
         """
         if self.dim ==2:
-            if psi is None:
-                psi = self.Q[0] +1j*self.Q[1]
+
+            psi = self.Q[0] +1j*self.Q[1]
 
             dt_psi = dt_Q[0] + 1j * dt_Q[1]
 
             return self.calc_defect_velocity_field([np.real(psi), np.imag(psi)],
                                                    [np.real(dt_psi), np.imag(dt_psi)])
 
-    def calc_defect_polarization_field(self):
+
+    def calc_disclination_polarization_field(self):
+        """Calculates the polarization field of the disclination in two dimensions
+
+        Args:
+            None
+        
+        Returns:
+            The polarization field (numpy.narray)
+        """
         ex = np.real(sp.fft.ifftn(1j*self.k[0]*self.Q_f[0] + 1j*self.k[1]*self.Q_f[1]))
         ey = np.real(sp.fft.ifftn(1j * self.k[0] * self.Q_f[1] - 1j * self.k[1] * self.Q_f[0]))
         return np.array([ex,ey])
 
     def calc_disclination_nodes_nem(self, dt_Q=None,polarization = None,charge_tolerance=None):
-        """
-        Calculate the positions and charges of vortex nodes based on the defect density.
+        """Calculates the positions and charges of disclination nodes based on the disclination density.
         
-        Input:
-            dt_Q (numpy.narray, optional): The time derivative of the order parameter. If not provided, the velocity of the vortex nodes will not be calculated.
+        Args:
+            dt_Q: The time derivative of the order parameter. If not provided, the velocity of the disclination nodes will not be calculated. (numpy.narray, optional)
         
-        Output:
-            list: A list of dictionaries representing the vortex nodes. Each dictionary contains the following keys:
-                  - 'position_index': The position index of the vortex node in the defect density array.
-                  - 'charge': The charge of the vortex node.
-                  - 'position': The position of the vortex node as a list [x, y].
-                  - 'velocity': The velocity of the vortex node as a list [vx, vy].
+        Returns:
+            A list of dictionaries representing the disclination nodes. Each dictionary contains the following keys:
+                  - 'position_index': The position index of the disclination node in the disclination density array.
+                  - 'charge': The charge of the disclination node.
+                  - 'position': The position of the disclination node as a list [x, y].
+                  - 'velocity': The velocity of the disclination node as a list [vx, vy].
         """
 
-        # Calculate defect density
+        # Calculate disclination density
         if self.dim == 2:
-            psi = self.Q[0] + 1j*self.Q[1]
+
             rho = self.calc_disclination_density_nematic()
 
             if dt_Q is not None:
-                velocity_field = self.calc_vortex_velocity_field(dt_Q, psi)
+                velocity_field = self.calc_disclination_velocity_field(dt_Q)
 
 
-            vortex_nodes = self.calc_defect_nodes(np.abs(rho))
-            for vortex in vortex_nodes:
-                vortex['charge'] = np.sign(rho[vortex['position_index']])
+            disclination_nodes = self.calc_defect_nodes(np.abs(rho))
+            for disclination in disclination_nodes:
+                disclination['charge'] = np.sign(rho[disclination['position_index']])
 
                 if dt_Q is not None:
-                    vortex['velocity'] = [velocity_field[0][vortex['position_index']],
-                                          velocity_field[1][vortex['position_index']]]
+                    disclination['velocity'] = [velocity_field[0][disclination['position_index']],
+                                          velocity_field[1][disclination['position_index']]]
                 else:
-                    vortex['velocity'] = [float('nan'), float('nan')]
+                    disclination['velocity'] = [float('nan'), float('nan')]
 
-                if vortex['charge'] >0 and polarization is not None:
-                    vortex['polarization'] = [polarization[0][vortex['position_index']]
-                        ,polarization[1][vortex['position_index']]]
+                if disclination['charge'] >0 and polarization is not None:
+                    disclination['polarization'] = [polarization[0][disclination['position_index']]
+                        ,polarization[1][disclination['position_index']]]
                 else:
-                    vortex['polarization'] = [float('nan'), float('nan')]
+                    disclination['polarization'] = [float('nan'), float('nan')]
 
         elif self.dim == 3:
-            #TODO Make sure that tangent vector is continous
             omega, Omega, T, trD = self.calc_disclination_density_decoupled()
-            vortex_nodes = self.calc_defect_nodes(omega,charge_tolerance=None)
 
-            for vortex in vortex_nodes:
+            disclination_nodes = self.calc_defect_nodes(omega,charge_tolerance=None)
+            position_list = []
 
-                tangent_vector = np.array([T[i][vortex['position_index']] for i in range(3)])
+            for disclination in disclination_nodes:
 
+                tangent_vector = np.array([T[i][disclination['position_index']] for i in range(3)])
+                rotation_vector = np.array([Omega[i][disclination['position_index']] for i in range(3)])
 
-        return vortex_nodes
+                for i in range(len(position_list)):
+                    pos = position_list[i]
+                    if np.sqrt(sum( (disclination['position'][i] -pos[i])**2 for i in range(self.dim) )) <  5*self.a0:
+                        tan_neight = disclination_nodes[i]['Tangent_vector']
+                        if np.sum((tan_neight[j] -tangent_vector[j] )**2 -(tan_neight[j] + tangent_vector[j])**2 for j in range(self.dim)) > 0:
 
-    def plot_disclination_nodes(self, vortex_nodes, ax=None):
-        """
-        Plots the discliation nodes in the given axes.
+                            tangent_vector = -1* tangent_vector
+                        break
 
-        Input:
-            vortex_nodes (list): A list of dictionaries representing the vortex nodes. Each dictionary contains the following keys:
-                                 - 'position': The position of the vortex node as a list [x, y].
-                                 - 'charge': The charge of the vortex node.
-                                 - 'velocity': The velocity of the vortex node as a list [vx, vy].
-            ax (Axes, optional): The axes to plot the vortex nodes on. If not provided, a new subplot will be created.
+                if np.sign(np.dot(tangent_vector, rotation_vector)) != np.sign(trD[disclination['position_index']]):
+                    rotation_vector = -1*rotation_vector
+
+                disclination['Tangent_vector'] = tangent_vector
+                disclination['Rotation_vector'] = rotation_vector
+                position_list.append(disclination['position'])
+
+
+
+        return disclination_nodes
+
+    def plot_disclination_nodes(self, disclination_nodes, **kwargs):
+        """Plots the discliation nodes in the given axes.
+
+        Args:
+            disclination_nodes: A list of dictionaries representing the disclination nodes. Each dictionary contains the following keys:
+                                 - 'position': The position of the disclination node as a list [x, y].
+                                 - 'position_index': The index of the position
+                                 - 'charge' (2D only): The charge of the disclination node.
+                                 - 'velocity' (currently 2D only): The velocity of the disclination
+                                 - 'polarization' (2D only): The polarization of the +1/2 disclinations
+                                 - 'Tangent_vector' (3D only): the tangent of the disclination line
+                                 - 'Rotation_vector' (3D only): the rotation vector of the disclination line
+            -**kwargs: Keyword arguments for the plot.
+                See https://comfitlib.com/ClassBaseSystem/
+                for a full list of keyword arguments.
 
-        Output:
-            matplotlib.axes.Axes: The axes on which the disclination nodes are plotted.
+        Returns:
+            The axes on which the disclination nodes are plotted. (matplotlib.axes.Axes: )
         """
 
+        # Check if an axis object is provided
+        fig = kwargs.get('fig', plt.gcf())
+        ax = kwargs.get('ax', None)
+
         if self.dim == 2:
 
             if ax == None:
+                fig.clf()
                 ax = plt.gcf().add_subplot(111)
 
             x_coords_pos = []
             y_coords_pos = []
 
             x_coords_neg = []
             y_coords_neg = []
@@ -796,28 +836,28 @@
             vy_coords_neg = []
 
             px_coords_pos = []
             py_coords_pos = []
 
 
 
-            for vortex in vortex_nodes:
+            for disclination in disclination_nodes:
 
-                if vortex['charge'] > 0:
-                    x_coords_pos.append(vortex['position'][0])
-                    y_coords_pos.append(vortex['position'][1])
-                    vx_coords_pos.append(vortex['velocity'][0])
-                    vy_coords_pos.append(vortex['velocity'][1])
-                    px_coords_pos.append(vortex['polarization'][0])
-                    py_coords_pos.append(vortex['polarization'][1])
+                if disclination['charge'] > 0:
+                    x_coords_pos.append(disclination['position'][0])
+                    y_coords_pos.append(disclination['position'][1])
+                    vx_coords_pos.append(disclination['velocity'][0])
+                    vy_coords_pos.append(disclination['velocity'][1])
+                    px_coords_pos.append(disclination['polarization'][0])
+                    py_coords_pos.append(disclination['polarization'][1])
                 else:
-                    x_coords_neg.append(vortex['position'][0])
-                    y_coords_neg.append(vortex['position'][1])
-                    vx_coords_neg.append(vortex['velocity'][0])
-                    vy_coords_neg.append(vortex['velocity'][1])
+                    x_coords_neg.append(disclination['position'][0])
+                    y_coords_neg.append(disclination['position'][1])
+                    vx_coords_neg.append(disclination['velocity'][0])
+                    vy_coords_neg.append(disclination['velocity'][1])
 
 
             # print(x_coords_pos,y_coords_pos)
             # print(x_coords_neg,y_coords_neg)
             ax.scatter(x_coords_pos, y_coords_pos, marker='+', color='red')
             ax.scatter(x_coords_neg, y_coords_neg, marker='*', color='blue')
             ax.quiver(x_coords_pos, y_coords_pos, vx_coords_pos, vy_coords_pos, color='black')
@@ -829,53 +869,202 @@
             ax.set_xlabel('$x/a_0$')
             ax.set_ylabel('$y/a_0$')
 
             ax.set_xlim([0, self.xmax-self.dx])
             ax.set_ylim([0, self.ymax-self.dy])
             return ax
 
+        elif self.dim == 3:
+            # Plotting options
+            quiver_scale = 2  # The scale of the quiver arrows
 
-    def plot_field_velocity_and_director(self, field, velocity, director, ax=None, colorbar=True, colormap='viridis',
-                                         cmax=None, cmin=None,
-                                         number_of_layers=1, hold=False):
-        """
-        Plot the field, velocity, and director in the given axes.
+            if ax == None:
+                plt.clf()
+                ax = plt.gcf().add_subplot(111, projection='3d')
+            x_coords = []
+            y_coords = []
+            z_coords = []
+
+            tx = []
+            ty = []
+            tz = []
+
+            Ox = []
+            Oy = []
+            Oz = []
+
+            for disclination in disclination_nodes:
+                x_coords.append(disclination['position'][0])
+                y_coords.append(disclination['position'][1])
+                z_coords.append(disclination['position'][2])
+
+                tx.append(disclination['Tangent_vector'][0])
+                ty.append(disclination['Tangent_vector'][1])
+                tz.append(disclination['Tangent_vector'][2])
+
+                Ox.append(disclination['Rotation_vector'][0])
+                Oy.append(disclination['Rotation_vector'][1])
+                Oz.append(disclination['Rotation_vector'][2])
+
+            tx = np.array(tx)
+            ty = np.array(ty)
+            tz = np.array(tz)
+
+            Ox = np.array(Ox)
+            Oy = np.array(Oy)
+            Oz = np.array(Oz)
+
+
+            # ax.scatter(x_coords, y_coords, z_coords, marker='o', color='black')
+            ax.quiver(x_coords, y_coords, z_coords, quiver_scale * tx, quiver_scale * ty, quiver_scale * tz,
+                      color='blue')
+            ax.quiver(x_coords, y_coords, z_coords, quiver_scale * Ox*0.75 , quiver_scale * Oy*0.75 ,
+                      quiver_scale * Oz*0.75, color='green')
 
-        Input:
+            ax.set_xlabel('$x/a_0$')
+            ax.set_ylabel('$y/a_0$')
+            ax.set_zlabel('$z/a_0$')
+
+            ax.set_xlim([0, self.xmax - self.dx])
+            ax.set_ylim([0, self.ymax - self.dy])
+            ax.set_zlim([0, self.zmax - self.dz])
+
+            ax.set_aspect('equal')
+            ax.grid(True)
+
+            return ax
+
+    def plot_field_velocity_and_director(self, field, velocity, director, **kwargs):
+        """Plot the fields, velocity, and director field in 2 dimensions
+
+        Args:
             field (ndarray): The field to be plotted.
             velocity (ndarray): The velocity to be plotted.
             director (ndarray): The director to be plotted.
-            ax (Axes, optional): The axes to plot the field, velocity, and director on. If not provided, a new subplot will be created.
-            colorbar (bool, optional): Whether to show the colorbar. Default is True.
-            colormap (str, optional): The colormap to use for plotting the field. Default is 'viridis'.
-            cmax (float, optional): The maximum value for the colorbar. If not provided, the maximum value of the field will be used.
-            cmin (float, optional): The minimum value for the colorbar. If not provided, the minimum value of the field will be used.
-            number_of_layers (int, optional): The number of layers in the plot. Default is 1.
-            hold (bool, optional): Whether to hold the plot. Default is False.
-
-        Output:
-            ax (Axes): The axes with the plotted field, velocity, and director.
+            **kwargs: Keyword arguments for the plot.
+                See https://comfitlib.com/ClassBaseSystem/
+                for a full list of keyword arguments.
+
+        Returns:
+            A tuple consisting of
+                - The figure
+                - The axes with the plotted field, velocity, and director. ax (Axes)
 
         Raises:
-            Exception: If the plotting function is not yet configured for dimensions other than 2.
-
-        Note: streamplot assumes xy indexing and not ij. I think it is suficient
-        just transpose the matrices before putting them in
+            Exception: If the dimension is other than 2.
         """
+        if field.dtype == bool:
+         field = field.astype(float)
+
+        # Check if the vector field is complex
+        if np.iscomplexobj(field):
+            print(
+                 "\033[91mWarning: the provided field was complex. This might be due to residual imaginary parts from the Fourier transform. The imaginary parts will be removed.\033[0m")
+            print('Max imaginary part: ', np.max(np.imag(field)))
+        field = np.real(field)
+
+        # Check if an axis object is provided
+        fig = kwargs.get('fig', plt.gcf())
+        ax = kwargs.get('ax', None)
+
+        # Kewyord arguments
+        colorbar = kwargs.get('colorbar', True)
+
+        # Extend the field if not a complete array is given
+        field = self.plot_tool_extend_field(field)
+
         if self.dim == 2:
+
+            # Keyword arguments particular to the 2D case
+            kwargs['grid'] = kwargs.get('grid', False)
+
             if ax == None:
+                fig.clf()
                 ax = plt.gcf().add_subplot(111)
+
+            colormap = kwargs.get('colormap', 'viridis')
+
+            if colormap == 'bluewhitered':
+                colormap = tool_colormap_bluewhitered()
+
+            elif colormap == 'sunburst':
+                colormap = tool_colormap_sunburst()
+            else:
+                colormap = plt.get_cmap(colormap)
+
             X, Y = np.meshgrid(self.x, self.y, indexing='ij')
-            if cmax is None:
-                cmax = np.max(field)
-            if cmin is None:
-                cmin = np.min(field)
-            cbar = ax.pcolormesh(X, Y, field, shading='gouraud', cmap=colormap, vmax=cmax, vmin=cmin)
-            plt.colorbar(cbar)
+            pcm = ax.pcolormesh(X / self.a0, Y / self.a0, field, shading='gouraud', cmap=colormap)
+
+            xlim = [self.xmin, self.xmax - self.dx]
+            ylim = [self.ymin, self.ymax - self.dy]
+
+            limits_provided = False
+            if 'xlim' in kwargs:
+                xlim = kwargs['xlim']
+                limits_provided = True
+            else:
+                if 'xmin' in kwargs:
+                    xlim[0] = kwargs['xmin']
+                    limits_provided = True
+
+                if 'xmax' in kwargs:
+                    xlim[1] = kwargs['xmax']
+                    limits_provided = True
+
+            if 'ylim' in kwargs:
+                ylim = kwargs['ylim']
+                limits_provided = True
+            else:
+                if 'ymin' in kwargs:
+                    ylim[0] = kwargs['ymin']
+                    limits_provided = True
+
+                if 'ymax' in kwargs:
+                    ylim[1] = kwargs['ymax']
+                    limits_provided = True
+            if limits_provided:
+                region_to_plot = np.zeros(self.dims).astype(bool)
+                region_to_plot[(xlim[0] <= X) * (X <= xlim[1]) * (ylim[0] <= Y) * (Y <= ylim[1])] = True
+                vlim = [np.min(field[region_to_plot]), np.max(field[region_to_plot])]
+
+            else:
+                vlim = [np.min(field), np.max(field)]
+
+            # Set the value limitses
+            if 'vlim' in kwargs:
+                vlim = kwargs['vlim']
+            else:
+                if 'vmin' in kwargs:
+                    vlim[0] = kwargs['vmin']
+                if 'vmax' in kwargs:
+                    vlim[1] = kwargs['vmax']
+
+            if vlim[1] - vlim[0] < 1e-10:
+                vlim = [vlim[0] - 0.05, vlim[1] + 0.05]
+
+            pcm.set_clim(vmin=vlim[0], vmax=vlim[1])
+
+            if 'vlim_symmetric' in kwargs:
+                vlim_symmetric = kwargs['vlim_symmetric']
+                if vlim_symmetric:
+                    cmax = abs(field).max()
+                    cmin = -cmax
+                    pcm.set_clim(vmin=cmin, vmax=cmax)
+
+            colorbar = kwargs.get('colorbar', True)
+
+            if colorbar:
+                cbar = plt.colorbar(pcm, ax=ax)
+
+
+
             ax.streamplot(X.T, Y.T, (velocity[0]).T, (velocity[1]).T, color='w')
             ax.quiver(X, Y, director[0], director[1], headwidth=0, scale=50)
             ax.quiver(X, Y, -director[0], -director[1], headwidth=0, scale=50)
             ax.set_aspect('equal')
-            return ax
 
         else:
-            raise Exception("This plotting function not yet configured for other dimension")
+            raise Exception("This plotting function is currently only implemented in 2D! ")
+
+        kwargs['ax'] = ax
+        self.plot_tool_set_axis_properties(**kwargs)
+        return fig, ax
```

### Comparing `comfit-1.4.2/comfit/models/quantum_mechanics.py` & `comfit-1.5.0/comfit/models/quantum_mechanics.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,26 @@
 from comfit.core.base_system import BaseSystem
 import matplotlib.pyplot as plt
 from comfit.tools.tool_colormaps import tool_colormap_angle, tool_colormap_bluewhitered
 import scipy as sp
 
 class QuantumMechanics(BaseSystem):
     def __init__(self, dimension, **kwargs):
-        """
-        Initializes a quamtum mechanics system evolving according to the Schrödinger equation
+        """Initializes a quamtum mechanics system evolving according to the Schrödinger equation
 
+        Args:
+            dimension: The dimension of the system.
+            **kwargs : dict, optional. Optional keyword arguments to set additional parameters. Same as BaseSystem
+                
+        Returns:
+            The system object representing the QuantumMechanics simulation.
+
+        Example:
+            qm = cf.QuantumMechanics(3,xRes=101,yRes=101,zRes=101)
+            Creates a BoseEinsteinCondensate system with 3 dimensions and a spatial resolution of 101.
         """
 
         # First initialize the BaseSystem class
         super().__init__(dimension, **kwargs)
 
         # Type of the system
         self.psi = None
@@ -23,22 +32,34 @@
         self.V_ext = 0  # External potential
 
         # If there are additional arguments provided, set them as attributes
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def __str__(self):
-        """
-        Output a string representation of the system
+        """Output a string representation of the system
+
+        Args:
+            None
+
+        Returns:
+            A string representation of the system
         """
         return 'QuantumMechanics'
 
     def conf_initial_condition_Gaussian(self,position=None,width=None, initial_velocity=None):
-        """
-        Set the initial condition to a Gaussian wavepacket.
+        """Set the initial condition to a Gaussian wavepacket.
+
+        Args:
+            position: The position of the wavepacket.
+            width: The width of the wavepacket.
+            initial_velocity: The initial velocity of the wavepacket.
+
+        Returns:
+            Configures self.psi and self.psi_f.
         """
 
         if position == None:
             position = self.rmid
         if width == None:
             width = self.xmax/10
     
@@ -58,18 +79,21 @@
                 v0 = initial_velocity
                 self.psi = self.psi * np.exp(1j * (v0[0] * self.x + v0[1]*self.y + v0[2]*self.z))
         
         self.psi_f = sp.fft.fftn(self.psi)
 
 
     def conf_harmonic_potential(self,trapping_strength=None):
-        """
-        Set the external potential to a harmonic trap with R_tf being the thomas fermi radius
-        :param R_tf:
-        :Output:
+        """Set the external potential to a harmonic trap with R_tf being the thomas fermi radius
+        
+        Args:
+            trapping_strength: The strength of the trapping potential.
+
+        Returns:
+            Configures self.V_ext.
         """
 
         if trapping_strength == None:
             trapping_strength = 1/(0.25*self.xmax)**2
 
 
         if self.dim ==1:
@@ -79,32 +103,38 @@
             return trapping_strength*(((self.x-self.xmid)**2) +((self.y-self.ymid)**2) )
         if self.dim == 3:
             return trapping_strength * (((self.x - self.xmid) ** 2)
                                            + ((self.y - self.ymid) ** 2)
                                            +((self.z - self.zmid) ** 2) )
 
     def conf_hydrogen_state(self,n,l,m):
-        """
-        Set the initial condition to a hydrogen state with quantum numbers n,l,m
+        """Set the initial condition to a hydrogen state with quantum numbers n,l,m
+
+        Args:
+            n: principal quantum number
+            l: azimuthal quantum number
+            m: magnetic quantum number
+
+        Returns:
+            Configures self.psi and self.psi_f.
         """
 
         self.psi = self.calc_hydrogen_state(n,l,m)
         self.psi_f = sp.fft.fftn(self.psi)
 
     def calc_hydrogen_state(self,n,l,m):
-        """
-        Calculate the hydrogen state with quantum numbers n,l,m
+        """Calculates the hydrogen state with quantum numbers n,l,m
 
-        Input:
+        Args:
             n: principal quantum number
             l: azimuthal quantum number
             m: magnetic quantum number
 
-        Output:
-            (np.ndarray): wavefunction
+        Returns:
+            Wavefunction of the hydrogen state. (np.ndarray)
         """
 
         if not self.dim == 3:
             raise(Exception('The hydrogen state is only defined in 3D'))
 
         r = np.sqrt(self.x**2 + self.y**2 + self.z**2)
         theta = np.arccos(self.z/r)
@@ -116,82 +146,43 @@
         
         return R*Y
 
     
 
     ## Calculation functions
     def calc_nonlinear_evolution_function_f(self,psi,t):
+        """Calculates the nonlinear evolution function f of the Schrödinger equation
+
+        Args:
+            psi: The wavefunction.
+            t: Time.
+        
+        Returns:
+            The nonlinear evolution function f.
+        """
 
         return sp.fft.fftn((1j) * (-self.V_ext) * psi)
 
 
     ## Time evolution functions
     def evolve_schrodinger(self,number_of_steps,method = 'ETD2RK'):
+        """Evolve the system according to the Schrödinger equation
+
+        Args:
+            number_of_steps: The number of steps to evolve the system.
+            method: The method to use for the time evolution. 
+        
+        Returns:
+            Evolves the system according to the Schrödinger equation.
+        """
         omega_f = -1j / 2 * self.calc_k2()
         if method == 'ETD2RK':
             integrating_factors_f = self.calc_evolution_integrating_factors_ETD2RK(omega_f)
             solver = self.evolve_ETD2RK_loop
         elif method == 'ETD4RK':
             integrating_factors_f = self.calc_evolution_integrating_factors_ETD4RK(omega_f)
             solver = self.evolve_ETD4RK_loop
         else:
             raise(Exception('This method is not implemented'))
         for n in range(number_of_steps):
             self.psi, self.psi_f = solver(integrating_factors_f, self.calc_nonlinear_evolution_function_f,
-                                                           self.psi, self.psi_f)
-
-
-    # Hamilton minimization functions
-
-    def calc_Hamiltonian(self):
-        integrand = -1/2*np.conj(self.psi)\
-            * sp.fft.ifftn(-self.calc_k2()*self.psi_f)\
-            + self.V_ext*abs(self.psi)**2
-        return self.calc_integrate_field(integrand)
-    
-    ## Plotting functions 
-    def plot(self, ylim=None):
-
-        if self.dim == 1:
-            plt.clf()
-            ax = plt.gcf().add_subplot(111)
-
-            cmap = tool_colormap_angle()
-
-
-            y = np.abs(self.psi) ** 2
-
-            c = np.angle(self.psi)
-
-            ax.plot(self.x,y,color='black')
-
-            if ylim is not None:
-                ax.set_ylim(0,ylim)
-
-
-            # Color in the graph based on the argument of the wavefunction
-            alpha_level=0.7
-
-            ax.fill_between([self.xmin,self.xmin+self.dx/2], [y[0],(y[0]+y[1])/2],
-                            color=cmap((c[0] + np.pi) / (2 * np.pi)), alpha=alpha_level,edgecolor='none')
-
-            for i in range(1,self.xRes-1):
-                ax.fill_between([self.x[i]-self.dx/2,self.x[i]+self.dx/2], [(y[i]+y[i-1])/2,(y[i]+y[i+1])/2],
-                                color = cmap((c[i] + np.pi) / (2 * np.pi)), alpha=alpha_level,edgecolor='none')
-
-            ax.fill_between([self.xmax-self.dx/2,self.xmax], [y[-1],(y[-1]+y[-2])/2],
-                            color=cmap((c[-1] + np.pi) / (2 * np.pi)), alpha=alpha_level,edgecolor='none')
-
-            ax.set_xlabel('$x/a_0$')
-            ax.set_ylabel('$|\psi|^2$')
-
-            sm = plt.cm.ScalarMappable(cmap=cmap)
-            cbar = plt.gcf().colorbar(sm, ax=ax)
-
-            #cbar.set_ticks(np.array([-np.pi, -2 * np.pi / 3, -np.pi / 3, 0, np.pi / 3, 2 * np.pi / 3, np.pi]))
-            cbar.set_ticks(np.array([0, 1/6, 2/6, 3/6, 4/6, 5/6, 1]))
-            cbar.set_ticklabels([r'$-\pi$', r'$-2\pi/3$', r'$-\pi/3$', r'$0$', r'$\pi/3$', r'$2\pi/3$', r'$\pi$'])
-            cbar.set_label('arg($\psi$)')
-
-
-            return ax
-    
+                                                           self.psi, self.psi_f)
```

### Comparing `comfit-1.4.2/comfit/tools/tool_colormaps.py` & `comfit-1.5.0/comfit/tools/tool_colormaps.py`

 * *Files identical despite different names*

### Comparing `comfit-1.4.2/comfit/tools/tool_create_orthonormal_triad.py` & `comfit-1.5.0/comfit/tools/tool_create_orthonormal_triad.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 def tool_create_orthonormal_triad(t):
     """
     This function creates an orthonormal triad given a vector t.
     The function first normalizes the input vector t, then it creates two orthogonal unit vectors e1 and e2.
     The vectors e1, e2, and the normalized t form an orthonormal triad.
 
-    Input:
+    Args:
     t : numpy array
         The input vector. It does not need to be a unit vector.
 
-    Output:
+    Returns:
     e1, e2, t : tuple of numpy arrays
         The orthonormal triad. Each element of the tuple is a numpy array representing a vector.
     """
     t = np.array(t)
 
     # Normalize the input vector
     t = t / np.linalg.norm(t)
```

### Comparing `comfit-1.4.2/comfit/tools/tool_math_functions.py` & `comfit-1.5.0/comfit/tools/tool_math_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         indices = np.array(args)
         counts = Counter(indices)
         prod = np.prod([factorial(count) for count in counts.values()])
         return 1 / prod
 
 def levi_civita_symbol(i, j, k):
     if {i, j, k} != {0, 1, 2}:
-        return 0  # Levi-Civita symbol is zero if indices are not 1, 2, 3
+        return 0  # Levi-Civita symbol is zero if indices are not 0, 1, 2
 
     if (i, j, k) in [(0, 1, 2), (1, 2, 0), (2, 0, 1)]:
         return 1  # Even permutation
     elif (i, j, k) in [(2, 1, 0), (0, 2, 1), (1, 0, 2)]:
         return -1  # Odd permutation
     else:
         return 0  # Repeated index
```

### Comparing `comfit-1.4.2/comfit/tools/tool_plot_manipulation_functions.py` & `comfit-1.5.0/comfit/tools/tool_plot_manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `comfit-1.4.2/tests/test_base_system.py` & `comfit-1.5.0/tests/test_base_system.py`

 * *Files identical despite different names*

### Comparing `comfit-1.4.2/tests/test_bose_einstein_condensate.py` & `comfit-1.5.0/tests/test_bose_einstein_condensate.py`

 * *Files identical despite different names*

### Comparing `comfit-1.4.2/tests/test_nematic_liquid_crystal.py` & `comfit-1.5.0/tests/test_nematic_liquid_crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,30 +32,32 @@
         # Check if nem.Q have approacjed the expected=
         S_0 = np.sqrt(nem.B)
         S,n = nem.calc_order_and_director()
         condition = np.allclose(S_0,S , atol=tolerance)
         self.assertTrue(condition, "Elements in nem.Q are not relaxed to the correct value")
 
     def test_no_flow_evolver_3D(self):
-        nem = cf.NematicLiquidCrystal(3, xRes=13, yRes=4,zRes=13,C =1)
-        np.random.seed(29820894)
-        nem.conf_initial_condition_ordered(noise_strength=2)
+        for i in range(10):
+            c = 2*np.random.rand()
+            nem = cf.NematicLiquidCrystal(3, xRes=13, yRes=4,zRes=13,C = c)
+            np.random.seed(29820894)
+            nem.conf_initial_condition_ordered(noise_strength=2)
 
-        nem.evolve_nematic_no_flow(300)
+            nem.evolve_nematic_no_flow(300)
 
 
-        # Set the tolerance for approximation
-        tolerance = 0.01
+            # Set the tolerance for approximation
+            tolerance = 0.01
 
-        # Check if all elements in  are approximately 1
-        S_0 =1/8* nem.C/nem.A + 1/2 * np.sqrt(nem.C**2 /(16*nem.A**2) + 3*nem.B)
+            # Check if all elements in  are approximately 1
+            S_0 =1/8* nem.C/nem.A + 1/2 * np.sqrt(nem.C**2 /(16*nem.A**2) + 3*nem.B)
 
-        S, n = nem.calc_order_and_director()
-        condition = np.allclose(S_0, S, atol=tolerance)
-        self.assertTrue(condition, "Elements in nem.Q are not relaxed to the correct value")
+            S, n = nem.calc_order_and_director()
+            condition = np.allclose(S_0, S, atol=tolerance)
+            self.assertTrue(condition, "Elements in nem.Q are not relaxed to the correct value")
 
 
 
     def test_nematic_evolver_with_defect_dipole(self):
         """Test the enm.evolve_nematic_no_flow"""
         nem = cf.NematicLiquidCrystal(2, xRes=31, yRes=31)
         nem.conf_insert_disclination_dipole(dipole_vector=[nem.xmax/3,0],
```

### Comparing `comfit-1.4.2/tests/test_phase_field_crystal.py` & `comfit-1.5.0/tests/test_phase_field_crystal.py`

 * *Files identical despite different names*

### Comparing `comfit-1.4.2/tests/test_quantum_mechanics.py` & `comfit-1.5.0/tests/test_quantum_mechanics.py`

 * *Files identical despite different names*

