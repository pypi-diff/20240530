# Comparing `tmp/napari_moltrack-0.0.1.tar.gz` & `tmp/napari_moltrack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.1.tar", last modified: Thu May 30 16:58:49 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.2.tar", last modified: Thu May 30 17:31:07 2024, max compression
```

## Comparing `napari_moltrack-0.0.1.tar` & `napari_moltrack-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.242232 napari_moltrack-0.0.1/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-30 16:58:49.242232 napari_moltrack-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.1/README.md
--rw-rw-rw-   0        0        0     3402 2024-05-29 16:36:17.000000 napari_moltrack-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 16:58:49.244268 napari_moltrack-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.161889 napari_moltrack-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.173927 napari_moltrack-0.0.1/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.173927 napari_moltrack-0.0.1/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.1/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    61681 2024-05-30 13:51:32.000000 napari_moltrack-0.0.1/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-29 16:15:26.000000 napari_moltrack-0.0.1/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.185611 napari_moltrack-0.0.1/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.1/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.1/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     6552 2024-05-30 16:54:29.000000 napari_moltrack-0.0.1/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.214232 napari_moltrack-0.0.1/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.1/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.1/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    13311 2024-05-30 12:41:31.000000 napari_moltrack-0.0.1/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.1/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    13341 2024-05-30 11:32:08.000000 napari_moltrack-0.0.1/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.1/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    34039 2024-05-30 16:52:33.000000 napari_moltrack-0.0.1/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.1/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    18504 2024-05-30 09:31:37.000000 napari_moltrack-0.0.1/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.1/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.1/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-30 16:58:49.232210 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 16:58:49.000000 napari_moltrack-0.0.1/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.162120 napari_moltrack-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.177741 napari_moltrack-0.0.2/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.193362 napari_moltrack-0.0.2/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.2/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    61681 2024-05-30 13:51:32.000000 napari_moltrack-0.0.2/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-05-30 17:30:58.000000 napari_moltrack-0.0.2/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.199895 napari_moltrack-0.0.2/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.2/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.2/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     6552 2024-05-30 16:54:29.000000 napari_moltrack-0.0.2/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.215547 napari_moltrack-0.0.2/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.2/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.2/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    13311 2024-05-30 12:41:31.000000 napari_moltrack-0.0.2/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     8893 2024-05-30 11:25:33.000000 napari_moltrack-0.0.2/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    13425 2024-05-30 17:25:19.000000 napari_moltrack-0.0.2/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.2/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    34039 2024-05-30 16:52:33.000000 napari_moltrack-0.0.2/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.2/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    18504 2024-05-30 09:31:37.000000 napari_moltrack-0.0.2/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4161 2024-05-30 10:54:17.000000 napari_moltrack-0.0.2/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.2/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-30 17:31:07.231171 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 17:31:07.000000 napari_moltrack-0.0.2/src/napari_moltrack.egg-info/top_level.txt
```

### Comparing `napari_moltrack-0.0.1/LICENSE` & `napari_moltrack-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/PKG-INFO` & `napari_moltrack-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.1/README.md` & `napari_moltrack-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/pyproject.toml` & `napari_moltrack-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 [tool.setuptools.dynamic]
 version = {attr = "moltrack.__init__.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-"*" = ["*.yaml"]
-
-
+"*" = ["*.yaml","*.dll"]
 
 [tool.black]
 line-length = 79
 target-version = ['py38', 'py39', 'py310']
 
 [tool.ruff]
 line-length = 79
```

### Comparing `napari_moltrack-0.0.1/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.2/src/moltrack/GUI/widget_ui.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.2/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/_widget.py` & `napari_moltrack-0.0.2/src/moltrack/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/import_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,33 @@
                     np_array[frame_index] = img_frame
 
                     progress = int(((frame_index + 1) / n_frames)*100)
                     progress_dict[index] = progress
 
         elif ext.lower() == ".fits":
 
+            time_start = time.time()
+
             with fits.open(path) as hdul:
 
+                shared_mem = dat["shared_image"]
+                np_array = np.ndarray(dat["image_shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
+
                 for frame_index in range(n_frames):
 
                     img_frame = hdul[0].data[frame_index]
 
-                    shared_mem = dat["shared_image"]
-                    np_array = np.ndarray(dat["image_shape"], dtype=dat["dtype"], buffer=shared_mem.buf)
                     np_array[frame_index] = img_frame
 
                     progress = int(((frame_index + 1) / n_frames)*100)
                     progress_dict[index] = progress
 
+            end_time = time.time()
+            print(f"Time taken: {end_time - time_start}")
+
     except:
         print(traceback.format_exc())
         pass
 
 
 
 
@@ -333,16 +339,14 @@
             else:
                 dataset_list = list(import_dict.keys())
 
                 for dataset_name in dataset_list:
                     dataset_dict = import_dict.pop(dataset_name)
                     self.dataset_dict[dataset_name] = dataset_dict
 
-            print(self.dataset_dict.keys())
-
         except:
             print(traceback.format_exc())
             pass
 
     def import_data(self, progress_callback=None, paths=[]):
 
         image_list, self.shared_images, import_dict = self.populate_import_lists(paths=paths)
```

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.2/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.1/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.2/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.1/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.2/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

