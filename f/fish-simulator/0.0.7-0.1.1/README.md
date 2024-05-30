# Comparing `tmp/fish_simulator-0.0.7.tar.gz` & `tmp/fish_simulator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fish_simulator-0.0.7.tar", last modified: Thu Aug 31 12:36:51 2023, max compression
+gzip compressed data, was "fish_simulator-0.1.1.tar", last modified: Thu May 30 21:19:16 2024, max compression
```

## Comparing `fish_simulator-0.0.7.tar` & `fish_simulator-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.367607 fish_simulator-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (999)     6148 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      631 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1357 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (999)     3078 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)    21198 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (999)      382 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (999)     1077 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2816 2023-08-31 12:36:51.367607 fish_simulator-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2124 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/fish_simulator/
--rw-r--r--   0 runner    (1001) docker     (999)      270 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1499 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/image_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/fish_simulator/png_template/
--rw-r--r--   0 runner    (1001) docker     (999)    30567 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/png_template/whole_larval_zf.png
--rw-r--r--   0 runner    (1001) docker     (999)     7791 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/simulator.py
--rw-r--r--   0 runner    (1001) docker     (999)     8612 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/tail_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/fish_simulator/template_img/
--rw-r--r--   0 runner    (1001) docker     (999)   155083 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/fish_head.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.367607 fish_simulator-0.0.7/fish_simulator/template_img/segs/
--rw-r--r--   0 runner    (1001) docker     (999)     3090 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/00.png
--rw-r--r--   0 runner    (1001) docker     (999)     2755 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/01.png
--rw-r--r--   0 runner    (1001) docker     (999)     3513 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/02.png
--rw-r--r--   0 runner    (1001) docker     (999)     2390 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/03.png
--rw-r--r--   0 runner    (1001) docker     (999)     2956 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/04.png
--rw-r--r--   0 runner    (1001) docker     (999)     2203 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/05.png
--rw-r--r--   0 runner    (1001) docker     (999)     1900 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/06.png
--rw-r--r--   0 runner    (1001) docker     (999)     3000 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/07.png
--rw-r--r--   0 runner    (1001) docker     (999)     2497 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/08.png
--rw-r--r--   0 runner    (1001) docker     (999)     3163 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/09.png
--rw-r--r--   0 runner    (1001) docker     (999)     1907 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/10.png
--rw-r--r--   0 runner    (1001) docker     (999)     3311 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/11.png
--rw-r--r--   0 runner    (1001) docker     (999)     2006 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/12.png
--rw-r--r--   0 runner    (1001) docker     (999)     2681 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/13.png
--rw-r--r--   0 runner    (1001) docker     (999)     1741 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/14.png
--rw-r--r--   0 runner    (1001) docker     (999)     2268 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/15.png
--rw-r--r--   0 runner    (1001) docker     (999)     2462 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/16.png
--rw-r--r--   0 runner    (1001) docker     (999)     2316 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/17.png
--rw-r--r--   0 runner    (1001) docker     (999)     1523 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/18.png
--rw-r--r--   0 runner    (1001) docker     (999)     2206 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/19.png
--rw-r--r--   0 runner    (1001) docker     (999)     2418 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/20.png
--rw-r--r--   0 runner    (1001) docker     (999)     2080 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/21.png
--rw-r--r--   0 runner    (1001) docker     (999)     2245 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/22.png
--rw-r--r--   0 runner    (1001) docker     (999)     2233 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/23.png
--rw-r--r--   0 runner    (1001) docker     (999)     1869 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/24.png
--rw-r--r--   0 runner    (1001) docker     (999)     2757 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/25.png
--rw-r--r--   0 runner    (1001) docker     (999)     1469 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/26.png
--rw-r--r--   0 runner    (1001) docker     (999)     1557 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/27.png
--rw-r--r--   0 runner    (1001) docker     (999)     2169 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/28.png
--rw-r--r--   0 runner    (1001) docker     (999)     1662 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/29.png
--rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/30.png
--rw-r--r--   0 runner    (1001) docker     (999)     1992 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/31.png
--rw-r--r--   0 runner    (1001) docker     (999)     1638 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/32.png
--rw-r--r--   0 runner    (1001) docker     (999)     1636 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/33.png
--rw-r--r--   0 runner    (1001) docker     (999)     1543 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/34.png
--rw-r--r--   0 runner    (1001) docker     (999)     1294 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/35.png
--rw-r--r--   0 runner    (1001) docker     (999)     1850 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/36.png
--rw-r--r--   0 runner    (1001) docker     (999)     2238 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/fish_simulator/template_img/segs/37.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.359607 fish_simulator-0.0.7/fish_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2816 2023-08-31 12:36:51.000000 fish_simulator-0.0.7/fish_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2159 2023-08-31 12:36:51.000000 fish_simulator-0.0.7/fish_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 12:36:51.000000 fish_simulator-0.0.7/fish_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       66 2023-08-31 12:36:51.000000 fish_simulator-0.0.7/fish_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-31 12:36:51.000000 fish_simulator-0.0.7/fish_simulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      697 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       52 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-31 12:36:51.367607 fish_simulator-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1375 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:36:51.367607 fish_simulator-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (999)     1972 2023-08-31 12:36:39.000000 fish_simulator-0.0.7/test/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.114037 fish_simulator-0.1.1/fish_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17595 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/fish_simulator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/fish_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 21:19:16.000000 fish_simulator-0.1.1/fish_simulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:19:16.118037 fish_simulator-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:19:16.114037 fish_simulator-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-30 21:19:09.000000 fish_simulator-0.1.1/test/test_methods.py
```

### Comparing `fish_simulator-0.0.7/LICENSE` & `fish_simulator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fish_simulator-0.0.7/fish_simulator/tail_transformation.py` & `fish_simulator-0.1.1/fish_simulator/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
         else:
             interpolator = interp1d(
                 distance, points[:id_first_nan, :], kind="linear", axis=0
             )
 
         curve = interpolator(alpha)
 
-        tail_x_interp[i_tp, : key_pnt_struc.n_segments+1] = curve[:, 0]
-        tail_y_interp[i_tp, : key_pnt_struc.n_segments+1] = curve[:, 1]
+        tail_x_interp[i_tp, : key_pnt_struc.n_segments + 1] = curve[:, 0]
+        tail_y_interp[i_tp, : key_pnt_struc.n_segments + 1] = curve[:, 1]
         # except Exception as e:
         #     print(f"Error {e} occurred.")
         #     print(f"Keypoint interpolation failed tp: {i_tp}")
 
     return tail_x_interp, tail_y_interp
```

### Comparing `fish_simulator-0.0.7/test/test_methods.py` & `fish_simulator-0.1.1/test/test_methods.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,55 @@
 """Unit test ImageLoader class functionality"""
 import unittest
 from pathlib import Path
 import numpy as np
-from fish_simulator import image_loading
+from fish_simulator import image_loader
 
 
 class TestImageLoader(unittest.TestCase):
     """Import class tester for ImageLoader"""
+
     def setUp(self):
-        """Instantiate default and constructed class
-        """
+        """Instantiate default and constructed class"""
         print("\nRunning setUp method...")
-        self.img_loader_default = image_loading.ImageLoader()
-        self.img_loader = image_loading.ImageLoader(
-            "./fish_simulator/template_img/segs"
-        )
+        self.img_loader_default = image_loader.ImageLoader()
+        self.img_loader = image_loader.ImageLoader(f"{Path(__file__).parents[1]}/fish_simulator/templates/template_img2/segs")
 
     def tearDown(self):
-        """Destruct test class
-        """
+        """Destruct test class"""
         print("Running tearDown method...")
 
     def test_default_dir_exists(self):
-        """Test if directories exist in repo
-        """
+        """Test if directories exist in repo"""
         print("Running test_default_dir_exists")
         print(self.img_loader_default.seg_dir)
+        print(self.img_loader.seg_dir)
         self.assertEqual(Path(self.img_loader.seg_dir).is_dir(), True)
         self.assertEqual(Path(self.img_loader_default.seg_dir).is_dir(), True)
 
     def test_finds_default_dir(self):
-        """Test the default directory is valid
-        """
+        """Test the default directory is valid"""
         print("Running test_default_dir is true")
         self.assertEqual(
-            "fish_simulator/template_img/segs"
-            in str(self.img_loader_default.seg_dir),
+            "fish_simulator/templates/template_img2/segs" in str(self.img_loader_default.seg_dir),
             True,
         )
 
     def test_all_segs_loaded(self):
-        """Check dimensions of segments loaded and dtype within list
-        """
+        """Check dimensions of segments loaded and dtype within list"""
         print("Running test_load_segment images...")
-        self.assertEqual(len(self.img_loader.load_segments()), 38)
+        self.assertEqual(len(self.img_loader.load_segments()), 48)
         self.assertEqual(
             all(
                 isinstance(seg_, np.ndarray) for seg_ in self.img_loader.load_segments()
             ),
             True,
         )
 
     def test_head_loaded(self):
-        """Test dimensions of loaded head
-        """
+        """Test dimensions of loaded head"""
         print("Running test_load_head image...")
-        self.assertEqual(self.img_loader.load_head().shape, (522, 836, 4))
+        self.assertEqual(self.img_loader.load_head().shape, (310, 576, 4))
 
 
 if __name__ == "__main__":
     unittest.main()
```

