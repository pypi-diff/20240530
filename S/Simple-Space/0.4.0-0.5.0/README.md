# Comparing `tmp/simple_space-0.4.0.tar.gz` & `tmp/simple_space-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.4.0.tar", last modified: Thu May 30 19:17:58 2024, max compression
+gzip compressed data, was "simple_space-0.5.0.tar", last modified: Thu May 30 21:23:31 2024, max compression
```

## Comparing `simple_space-0.4.0.tar` & `simple_space-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.4.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 19:17:58.877098 simple_space-0.4.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.4.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.873098 simple_space-0.4.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.4.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.4.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.4.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.4.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3929 2024-05-30 19:11:27.000000 simple_space-0.4.0/SimpleS/Points/dim2.py
--rw-rw-r--   0 user      (1000) user      (1000)     8665 2024-05-30 19:11:48.000000 simple_space-0.4.0/SimpleS/Points/dim3.py
--rw-rw-r--   0 user      (1000) user      (1000)       46 2024-05-30 19:17:29.000000 simple_space-0.4.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.4.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 19:17:52.000000 simple_space-0.4.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 19:17:58.877098 simple_space-0.4.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:23:31.664203 simple_space-0.5.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.5.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 21:23:31.664203 simple_space-0.5.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.5.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:23:31.660203 simple_space-0.5.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:23:31.660203 simple_space-0.5.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.5.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.5.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.5.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:23:31.660203 simple_space-0.5.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.5.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4748 2024-05-30 21:22:31.000000 simple_space-0.5.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8665 2024-05-30 19:11:48.000000 simple_space-0.5.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)       47 2024-05-30 21:23:09.000000 simple_space-0.5.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.5.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 21:23:31.664203 simple_space-0.5.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 21:23:31.000000 simple_space-0.5.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 21:23:31.000000 simple_space-0.5.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 21:23:31.000000 simple_space-0.5.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 21:23:31.000000 simple_space-0.5.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 21:23:31.000000 simple_space-0.5.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 21:23:19.000000 simple_space-0.5.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 21:23:31.664203 simple_space-0.5.0/setup.cfg
```

### Comparing `simple_space-0.4.0/LICENSE` & `simple_space-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/PKG-INFO` & `simple_space-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.4.0/README.md` & `simple_space-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/SimpleS/ImageRelated/basics.py` & `simple_space-0.5.0/SimpleS/ImageRelated/basics.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-0.5.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/SimpleS/Points/dim2.py` & `simple_space-0.5.0/SimpleS/Points/dim2.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,45 @@
 from SimpleS.utils import save_path_generator
 import scipy.ndimage as ndi
 from skimage import img_as_ubyte
 from skimage.morphology import skeletonize
 
 
 
-def create_flat_image_2d(size=(750, 750), color_mode='RGB', color = 'White',return_ = True, save = False, save_path = None, file_name = None):
+
+def rotate_points(points, theta=0, axis=None):
+    """Rotate or reflect 2D points by theta degrees around the origin or inverting the specified axis."""
+    points = np.asarray(points)
+    if points.shape[1] != 2:
+        raise ValueError("Points should be in shape (n, 2)")
+    if axis == 'x':
+        # invert the y-coordinates.
+        rot_matrix = np.array([
+            [1, 0],
+            [0, -1]
+        ])
+    elif axis == 'y':
+        # invert the x-coordinates.
+        rot_matrix = np.array([
+            [-1, 0],
+            [0, 1]
+        ])
+    else:
+        # rotation around the origin by theta.
+        theta = np.radians(theta)
+        rot_matrix = np.array([
+            [np.cos(theta), -np.sin(theta)],
+            [np.sin(theta), np.cos(theta)]
+        ])
+    return np.dot(points, rot_matrix.T)
+
+
+
+
+def create_flat_image(size=(750, 750), color_mode='RGB', color = 'White',return_ = True, save = False, save_path = None, file_name = None):
         """
         Create a white image of the specified size and color mode.
         Parameters:
         size (tuple): The dimensions of the image (width, height).
         color_mode (str): The color mode of the image, either 'RGB' or 'Gray'.
         Returns:
         numpy.ndarray: The created white image.
```

### Comparing `simple_space-0.4.0/SimpleS/Points/dim3.py` & `simple_space-0.5.0/SimpleS/Points/dim3.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/SimpleS/utils.py` & `simple_space-0.5.0/SimpleS/utils.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.4.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-0.5.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.4.0/pyproject.toml` & `simple_space-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

