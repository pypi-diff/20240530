# Comparing `tmp/simple_space-0.3.0.tar.gz` & `tmp/simple_space-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.3.0.tar", last modified: Thu May 30 18:56:06 2024, max compression
+gzip compressed data, was "simple_space-0.4.0.tar", last modified: Thu May 30 19:17:58 2024, max compression
```

## Comparing `simple_space-0.3.0.tar` & `simple_space-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.817522 simple_space-0.3.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.3.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:56:06.817522 simple_space-0.3.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     9972 2024-05-30 18:05:04.000000 simple_space-0.3.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.3.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.3.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.3.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.3.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    12512 2024-05-30 15:58:52.000000 simple_space-0.3.0/SimpleS/Points/dimentions.py
--rw-rw-r--   0 user      (1000) user      (1000)       88 2024-05-30 18:54:16.000000 simple_space-0.3.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.3.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.817522 simple_space-0.3.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      405 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 18:54:38.000000 simple_space-0.3.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 18:56:06.817522 simple_space-0.3.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.4.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 19:17:58.877098 simple_space-0.4.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.4.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.873098 simple_space-0.4.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.4.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.4.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.4.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.4.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3929 2024-05-30 19:11:27.000000 simple_space-0.4.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8665 2024-05-30 19:11:48.000000 simple_space-0.4.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2024-05-30 19:17:29.000000 simple_space-0.4.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.4.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 19:17:58.877098 simple_space-0.4.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 19:17:58.000000 simple_space-0.4.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 19:17:52.000000 simple_space-0.4.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 19:17:58.877098 simple_space-0.4.0/setup.cfg
```

### Comparing `simple_space-0.3.0/LICENSE` & `simple_space-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.3.0/PKG-INFO` & `simple_space-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,15 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [Dim3 Class](#dim3-class)
+  - [dim3](#dim3)
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -67,70 +67,69 @@
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
-    - dimentions.py:
-     Contains the Dim3 and Dim2 classes for 3D and 2D point data processing and visualization.
+    - dim3.py:
+     Contains functions for 3D point data processing and visualization.
+    - dim2.py:
+     Contains some simple and basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## Dim3 Class
+## dim3
 
-The Dim3 class offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
 #### Initializing the Class
 
 ```python
 
-from SimpleS.Points.dimentions import Dim3
+from SimpleS.Points import dim3
 
-# Or even :
-
-from SimpleS import Dim3
 ```
 ```python
 # But I recommend You Simply Use this one:
 
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside Dim3 class without any initialize word;
+# This one Lets you use all the functions inside dim3 script without any initialize word;
 # FOR EXAMPLE:
 
-Dim3.rotate_points()
+dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_3d_points()
+rotate_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
-from SimpleS import Dim3
+from SimpleS.Points import dim3
 
-dir(Dim3)
+dir(dim3)
 ```
-This will show you the names of all functions inside the Dim3 class.
+This will show you the names of all functions inside the dim3 script.
 
 After that, we will return to our simpler method:
 
 ```python
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 ```
 
 #### Rotating 3D Points
 
 ```python
 rotated_points = rotate_points(points, 45, 'z')
 ```
```

### Comparing `simple_space-0.3.0/README.md` & `simple_space-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [Dim3 Class](#dim3-class)
+  - [dim3](#dim3)
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -40,70 +40,69 @@
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
-    - dimentions.py:
-     Contains the Dim3 and Dim2 classes for 3D and 2D point data processing and visualization.
+    - dim3.py:
+     Contains functions for 3D point data processing and visualization.
+    - dim2.py:
+     Contains some simple and basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## Dim3 Class
+## dim3
 
-The Dim3 class offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
 #### Initializing the Class
 
 ```python
 
-from SimpleS.Points.dimentions import Dim3
+from SimpleS.Points import dim3
 
-# Or even :
-
-from SimpleS import Dim3
 ```
 ```python
 # But I recommend You Simply Use this one:
 
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside Dim3 class without any initialize word;
+# This one Lets you use all the functions inside dim3 script without any initialize word;
 # FOR EXAMPLE:
 
-Dim3.rotate_points()
+dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_3d_points()
+rotate_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
-from SimpleS import Dim3
+from SimpleS.Points import dim3
 
-dir(Dim3)
+dir(dim3)
 ```
-This will show you the names of all functions inside the Dim3 class.
+This will show you the names of all functions inside the dim3 script.
 
 After that, we will return to our simpler method:
 
 ```python
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 ```
 
 #### Rotating 3D Points
 
 ```python
 rotated_points = rotate_points(points, 45, 'z')
 ```
```

### Comparing `simple_space-0.3.0/SimpleS/ImageRelated/basics.py` & `simple_space-0.4.0/SimpleS/ImageRelated/basics.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.3.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-0.4.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.3.0/SimpleS/utils.py` & `simple_space-0.4.0/SimpleS/utils.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.3.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-0.4.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,15 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [Dim3 Class](#dim3-class)
+  - [dim3](#dim3)
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -67,70 +67,69 @@
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
-    - dimentions.py:
-     Contains the Dim3 and Dim2 classes for 3D and 2D point data processing and visualization.
+    - dim3.py:
+     Contains functions for 3D point data processing and visualization.
+    - dim2.py:
+     Contains some simple and basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## Dim3 Class
+## dim3
 
-The Dim3 class offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
 #### Initializing the Class
 
 ```python
 
-from SimpleS.Points.dimentions import Dim3
+from SimpleS.Points import dim3
 
-# Or even :
-
-from SimpleS import Dim3
 ```
 ```python
 # But I recommend You Simply Use this one:
 
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside Dim3 class without any initialize word;
+# This one Lets you use all the functions inside dim3 script without any initialize word;
 # FOR EXAMPLE:
 
-Dim3.rotate_points()
+dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_3d_points()
+rotate_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
-from SimpleS import Dim3
+from SimpleS.Points import dim3
 
-dir(Dim3)
+dir(dim3)
 ```
-This will show you the names of all functions inside the Dim3 class.
+This will show you the names of all functions inside the dim3 script.
 
 After that, we will return to our simpler method:
 
 ```python
-from SimpleS.Dim3 import *
+from SimpleS.Points.dim3 import *
 ```
 
 #### Rotating 3D Points
 
 ```python
 rotated_points = rotate_points(points, 45, 'z')
 ```
```

### Comparing `simple_space-0.3.0/pyproject.toml` & `simple_space-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

