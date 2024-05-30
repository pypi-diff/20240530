# Comparing `tmp/matsubplots-1.2.0.tar.gz` & `tmp/matsubplots-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matsubplots-1.2.0.tar", last modified: Sun May 12 01:12:05 2024, max compression
+gzip compressed data, was "matsubplots-1.2.1.tar", last modified: Thu May 30 17:45:55 2024, max compression
```

## Comparing `matsubplots-1.2.0.tar` & `matsubplots-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.730215 matsubplots-1.2.0/
--rw-rw-rw-   0        0        0     1089 2024-05-12 01:10:31.000000 matsubplots-1.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     1274 2024-05-12 01:12:05.728212 matsubplots-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-12 01:10:31.000000 matsubplots-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.682201 matsubplots-1.2.0/matsubplots/
--rw-rw-rw-   0        0        0      166 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/matsubplots.py
--rw-rw-rw-   0        0        0       23 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/version.py
--rw-rw-rw-   0        0        0     9005 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/viewers.py
-drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.725186 matsubplots-1.2.0/matsubplots.egg-info/
--rw-rw-rw-   0        0        0     1274 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      312 2024-05-12 01:12:05.733899 matsubplots-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-12 01:10:31.000000 matsubplots-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:45:55.034251 matsubplots-1.2.1/
+-rw-rw-rw-   0        0        0     1089 2024-05-30 17:44:18.000000 matsubplots-1.2.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1274 2024-05-30 17:45:55.034251 matsubplots-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-30 17:44:18.000000 matsubplots-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:45:54.997654 matsubplots-1.2.1/matsubplots/
+-rw-rw-rw-   0        0        0      166 2024-05-30 17:44:18.000000 matsubplots-1.2.1/matsubplots/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-05-30 17:44:18.000000 matsubplots-1.2.1/matsubplots/matsubplots.py
+-rw-rw-rw-   0        0        0       23 2024-05-30 17:44:18.000000 matsubplots-1.2.1/matsubplots/version.py
+-rw-rw-rw-   0        0        0     9242 2024-05-30 17:44:18.000000 matsubplots-1.2.1/matsubplots/viewers.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:45:55.034251 matsubplots-1.2.1/matsubplots.egg-info/
+-rw-rw-rw-   0        0        0     1274 2024-05-30 17:45:54.000000 matsubplots-1.2.1/matsubplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-30 17:45:54.000000 matsubplots-1.2.1/matsubplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:45:54.000000 matsubplots-1.2.1/matsubplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 17:45:54.000000 matsubplots-1.2.1/matsubplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 17:45:54.000000 matsubplots-1.2.1/matsubplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      312 2024-05-30 17:45:55.044342 matsubplots-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-30 17:44:18.000000 matsubplots-1.2.1/setup.py
```

### Comparing `matsubplots-1.2.0/LICENSE.md` & `matsubplots-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.2.0/PKG-INFO` & `matsubplots-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.2.0
+Version: 1.2.1
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.2.0/README.md` & `matsubplots-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.2.0/matsubplots/matsubplots.py` & `matsubplots-1.2.1/matsubplots/matsubplots.py`

 * *Files identical despite different names*

### Comparing `matsubplots-1.2.0/matsubplots/viewers.py` & `matsubplots-1.2.1/matsubplots/viewers.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,68 +13,76 @@
 
 class OrthoView:
 
     alignments = (0, 0), (0, 1), (1, 1)
     colors = '#ff0000', '#00ff00', '#ffff00'
     indices = (1, 2), (0, 2), (0, 1)
 
-    def __init__(self, axs, image, spacing=(1,1,1), slab_thickness=None, slab_func=np.mean, reposition=True, **kwargs):
+    def __init__(self, axs, image, spacing=(1,1,1), reposition=True, **kwargs):
         axs = np.asarray(axs)
         image = np.asarray(image)
         spacing = np.asarray(spacing)
         if not (axs.size == image.ndim == spacing.size == 3):
             raise ValueError('Expected a 3D image, 3 axes, and 3 values for spacing')
         bounds = []
         for i, ax in enumerate(axs.ravel()):
             j = image.shape[i] // 2
-            thickness = 1 if slab_thickness is None else round(slab_thickness / spacing[i])
-            j0 = np.maximum(j - thickness // 2, 0)
-            j1 = j - (-thickness // 2)
-            slice_ = slab_func(np.rollaxis(image, i)[j0:j1], axis=0)
             aspect = np.divide(*spacing[::-1][np.arange(spacing.size) != i])
             bounds.append([])
             bounds[-1].append(ax.get_position().bounds)
-            im = ax.imshow(slice_, aspect=aspect, **kwargs)
+            im = ax.imshow(np.rollaxis(image, i)[j], aspect=aspect, **kwargs)
             bounds[-1].append(ax.get_position().bounds)
             if hasattr(ax, 'cax'):
                 ax.get_figure().colorbar(im, cax=ax.cax)
         crosshairs = [[
             axs[i].axhline(image.shape[x]//2, lw=1, c=self.colors[x], visible=False),
             axs[i].axvline(image.shape[y]//2, lw=1, c=self.colors[y], visible=False)]
             for i, (x,y) in enumerate(self.indices)]
         self.axs = axs
         self.image = image
         self.spacing = spacing
         self._crosshairs = crosshairs
         if reposition:
             self._reposition(axs, bounds)
+        self.xyz()
 
     def crosshairs(self, toggle=None):
         if toggle is None:
             toggle = not self._crosshairs[0][0].get_visible()
         default_color = self.axs[0].get_xaxis().get_label().get_color()
         for i, crosshairs in enumerate(self._crosshairs):
             for line in crosshairs:
                 line.set_visible(toggle)
             for spine in self.axs[i].spines.values():
                 spine.set_edgecolor(self.colors[i] if toggle else default_color)
 
-    def ijk(self, i, j, k, crosshairs=None):
+    def ijk(self, i=None, j=None, k=None, crosshairs=None, **kwargs):
         for index, value in enumerate((i, j, k)):
-            self._scroll(index, value)
+            if value is None:
+                value = self.image.shape[index] // 2
+            self._scroll(index, value, **kwargs)
         if crosshairs is not None:
             self.crosshairs(crosshairs)
 
-    def xyz(self, x, y, z, crosshairs=None):
+    def xyz(self, x=0, y=0, z=0, **kwargs):
         xyz = x, y, z
         ijk = [round(xyz[::-1][i] / self.spacing[::-1][i] + (self.image.shape[i] - 1) / 2) for i in range(3)]
-        self.ijk(*ijk, crosshairs=crosshairs)
+        self.ijk(*ijk, **kwargs)
 
-    def _scroll(self, index, value):
-        self.axs[index].images[0].set_data(np.rollaxis(self.image, index)[value])
+    def _scroll(self, index, value, thickness=None, func=np.max):
+        if thickness is None:
+            i0, i1 = value, value + 1
+        elif np.isinf(thickness):
+            i0, i1 = None, None
+        else:
+            thickness = round(thickness / self.spacing[::-1][index])
+            i0 = np.maximum(value - thickness // 2, 0)
+            i1 = value - (-thickness // 2)
+        slab = func(np.rollaxis(self.image, index)[i0:i1], axis=0)
+        self.axs[index].images[-1].set_data(slab)
         for i, alignment in zip(self.indices[index], self.alignments[index]):
             getattr(self._crosshairs[i][alignment], 'set_ydata' if alignment == 0 else 'set_xdata')([value, value])
 
     @staticmethod
     def _reposition(axs, bounds):
         _, _, w00, _ = bounds[0][0]
         l01, b01, w01, h01 = bounds[0][1]
```

### Comparing `matsubplots-1.2.0/matsubplots.egg-info/PKG-INFO` & `matsubplots-1.2.1/matsubplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.2.0
+Version: 1.2.1
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.2.0/setup.py` & `matsubplots-1.2.1/setup.py`

 * *Files identical despite different names*

