# Comparing `tmp/comseg-0.0.8.tar.gz` & `tmp/comseg-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comseg-0.0.8.tar", last modified: Tue May 28 19:17:20 2024, max compression
+gzip compressed data, was "comseg-0.1.tar", last modified: Thu May 30 14:03:26 2024, max compression
```

## Comparing `comseg-0.0.8.tar` & `comseg-0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.0.8/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)     1235 2024-05-28 19:17:20.677910 comseg-0.0.8/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      800 2024-05-28 17:16:59.000000 comseg-0.0.8/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      513 2024-05-28 17:10:57.000000 comseg-0.0.8/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)      374 2024-05-28 17:08:31.000000 comseg-0.0.8/requirements.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-28 19:17:20.677910 comseg-0.0.8/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.673910 comseg-0.0.8/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/ComSeg.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1235 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-28 19:17:20.000000 comseg-0.0.8/src/ComSeg.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.0.8/src/__init__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/comseg/
--rw-rw-r--   0 tom       (1000) tom       (1000)      405 2024-05-15 12:21:09.000000 comseg-0.0.8/src/comseg/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18288 2024-05-15 12:06:26.000000 comseg-0.0.8/src/comseg/clustering.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18324 2024-05-28 17:22:36.000000 comseg-0.0.8/src/comseg/dataset.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    23616 2024-05-28 18:07:40.000000 comseg-0.0.8/src/comseg/dictionary.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    40561 2024-05-28 19:11:45.000000 comseg-0.0.8/src/comseg/model.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-28 19:17:20.677910 comseg-0.0.8/src/comseg/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.0.8/src/comseg/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    18897 2024-05-27 07:57:03.000000 comseg-0.0.8/src/comseg/utils/custom_louvain.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.0.8/src/comseg/utils/plot.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.0.8/src/comseg/utils/preprocessing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.0.8/src/comseg/utils/utils_graph.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1056 2023-10-04 17:16:12.000000 comseg-0.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1233 2024-05-30 14:03:26.884800 comseg-0.1/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      800 2024-05-28 17:16:59.000000 comseg-0.1/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      511 2024-05-30 13:59:02.000000 comseg-0.1/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)      374 2024-05-28 17:08:31.000000 comseg-0.1/requirements.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-05-30 14:03:26.888800 comseg-0.1/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/ComSeg.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1233 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      471 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       16 2024-05-30 14:03:26.000000 comseg-0.1/src/ComSeg.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        9 2024-02-13 12:19:38.000000 comseg-0.1/src/__init__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/comseg/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      403 2024-05-30 13:59:37.000000 comseg-0.1/src/comseg/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18288 2024-05-15 12:06:26.000000 comseg-0.1/src/comseg/clustering.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20754 2024-05-30 13:50:27.000000 comseg-0.1/src/comseg/dataset.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23470 2024-05-30 13:54:32.000000 comseg-0.1/src/comseg/dictionary.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    40560 2024-05-30 13:15:59.000000 comseg-0.1/src/comseg/model.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-05-30 14:03:26.884800 comseg-0.1/src/comseg/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-08-02 11:20:30.000000 comseg-0.1/src/comseg/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    18897 2024-05-27 07:57:03.000000 comseg-0.1/src/comseg/utils/custom_louvain.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1887 2023-10-03 13:00:25.000000 comseg-0.1/src/comseg/utils/plot.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8640 2023-11-21 18:48:35.000000 comseg-0.1/src/comseg/utils/preprocessing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3292 2023-10-25 14:42:29.000000 comseg-0.1/src/comseg/utils/utils_graph.py
```

### Comparing `comseg-0.0.8/LICENSE` & `comseg-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/PKG-INFO` & `comseg-0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.0.8
+Version: 0.1
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `comseg-0.0.8/README.md` & `comseg-0.1/README.md`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/src/ComSeg.egg-info/PKG-INFO` & `comseg-0.1/src/ComSeg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComSeg
-Version: 0.0.8
+Version: 0.1
 Summary: single cell RNA profiling analysis of imaging-based spatial transcriptomics data
 Author-email: Thomas Defard <thomas.defard@mines-paristech.fr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `comseg-0.0.8/src/comseg/clustering.py` & `comseg-0.1/src/comseg/clustering.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/src/comseg/dataset.py` & `comseg-0.1/src/comseg/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 
-import os
-import sys
-import networkx as nx
 import numpy as np
 
 import scipy
 import scipy.sparse as sp
 import tifffile
 
 import pandas as pd
 from scipy.stats import hypergeom
 from sklearn.neighbors import NearestNeighbors
 from pathlib import Path
-from sklearn.neighbors import radius_neighbors_graph
 #from processing_seg import full_df
 from tqdm import tqdm
-from skimage import measure
 ### dataset class
 from .utils.preprocessing import compute_dict_centroid
 
 
 
 
 class ComSegDataset():
@@ -36,50 +31,87 @@
 
     def __init__(self,
         path_dataset_folder,
         path_to_mask_prior = None,
         mask_file_extension = ".tiff",
         dict_scale={"x": 0.103, 'y': 0.103, "z": 0.3},
         mean_cell_diameter = 15,
-       gene_column = "gene"):
+        gene_column = "gene",
+        image_csv_files : list = None,
+        centroid_csv_files : list = None,
+        path_cell_centroid = None,
+        centroid_csv_key={"x": "x", "y": "y", "z": "z", "cell_index": "cell"}
+                 ):
 
         """
         :param path_dataset_folder: path to the folder containing the csv files
         :type path_dataset_folder: str
         :param path_to_mask_prior: path to the folder containing the mask priors. They must have the same name as the corresponding csv files
         :type path_to_mask_prior:  str
         :param mask_file_extension: file extension of the mask priors
         :default mask_file_extension: ".tiff"
         :param dict_scale: dictionary containing the pixel/voxel size of the images in µm default is {"x": 0.103, 'y': 0.103, "z": 0.3}
         :type dict_scale: dict
         :param mean_cell_diameter: the expected mean cell diameter in µm default is 15µm
         :type mean_cell_diameter: float
+        :param gene_column: name of the column containing the gene name in the csv files
+        :type gene_column: str
+        :param image_names_csv_file: list of image name as csv_file to consider in the dataset if None consider all the csv files in the folder
+        :type image_names_csv_file: list
+        :param centroid_name: list of the centroid as to be in the same order as the image_names_csv_file
+        :type centroid_name: list
         """
 
         self.path_dataset_folder = Path(path_dataset_folder)
         if path_to_mask_prior is not None:
             self.path_to_mask_prior = Path(path_to_mask_prior)
         else:
             self.path_to_mask_prior = None
         self.mask_file_extension = mask_file_extension
-        self.path_image_dict = {}
+        self.dict_scale = dict_scale
+        self.mean_cell_diameter = mean_cell_diameter
         self.gene_column = gene_column
-
+        self.path_image_dict = {}
         unique_gene = []
-        for image_path_df in self.path_dataset_folder.glob(f'*.csv'):
-            print(f"add {image_path_df.stem}")
-            self.path_image_dict[image_path_df.stem] = image_path_df
-            unique_gene += list(pd.read_csv(self.path_image_dict[image_path_df.stem])[self.gene_column].unique())
+        self.image_csv_files = image_csv_files
+        if image_csv_files is not None:
+            for image_name in image_csv_files:
+                image_path_df = Path(path_dataset_folder) / (image_name)
+                ## check if the csv file exists
+                assert image_path_df.exists(), f"{image_name} not found in the dataset folder {path_dataset_folder}"
+                self.path_image_dict[image_path_df.stem] = self.path_dataset_folder / (image_name)
+                unique_gene += list(pd.read_csv(self.path_image_dict[image_path_df.stem])[self.gene_column].unique())
+        else:
+            for image_path_df in self.path_dataset_folder.glob(f'*.csv'):
+                print(f"add {image_path_df.stem}")
+                self.path_image_dict[image_path_df.stem] = image_path_df
+                unique_gene += list(pd.read_csv(self.path_image_dict[image_path_df.stem])[self.gene_column].unique())
         if len(self.path_image_dict) == 0:
             raise ValueError(f"no csv file found in the dataset folder {self.path_dataset_folder}")
         self.list_index = list(self.path_image_dict.keys())
         self.selected_genes = np.unique(unique_gene)
-        self.dict_scale = dict_scale
-        self.dict_centroid = None
-        self.mean_cell_diameter = mean_cell_diameter
+        self.centroid_csv_files = centroid_csv_files
+        if self.centroid_csv_files is not None:
+            assert len(self.centroid_csv_files) == len(self.list_index), "centroid_file_name should have the same length as image_names_csv_file"
+            self.dict_centroid = {}
+            for i in range(len(self.centroid_csv_files)):
+                self.dict_centroid[self.list_index[i]] = self.centroid_csv_files[i]
+
+                df_centroid = pd.read_csv(Path(path_cell_centroid) / (self.centroid_csv_files[i]))
+                x_list = list(df_centroid[centroid_csv_key["x"]])
+                y_list = list(df_centroid["y"])
+                if centroid_csv_key["z"] in df_centroid.columns:
+                    z_list = list(df_centroid["z"])
+                cell_list = list(df_centroid[centroid_csv_key["cell_index"]])
+                if centroid_csv_key["z"] in df_centroid.columns:
+                    self.dict_centroid[self.list_index[i]] = {cell_list[i]: np.array([z_list[i], y_list[i], x_list[i]])
+                                          for i in range(len(cell_list))}
+                else:
+                    self.dict_centroid[self.list_index[i]] = {cell_list[i]: {"x": x_list[i], "y": y_list[i]} for i in range(len(cell_list))}
+                self.dict_centroid[self.list_index[i]]
 
     def __getitem__(self, key):
         if isinstance(key, int):
             return pd.read_csv(self.path_image_dict[self.list_index[key]])
         elif isinstance(key, str):
             return pd.read_csv(self.path_image_dict[key])
         return self.path_dataset_folder[key]
```

### Comparing `comseg-0.0.8/src/comseg/dictionary.py` & `comseg-0.1/src/comseg/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,17 @@
 
 
 #%%
 
 
 
 import pandas as pd
-import os
-import sys
+
 from tqdm import tqdm
 import anndata as ad
-#from model import ComSegGraph
-#import clustering
-#from . import clustering ## for dev mode
-#import model
-#import clustering
 import pickle
 from .clustering import InSituClustering
 from .model import ComSegGraph
 from pathlib import Path
 import numpy as np
 
 __all__ = ["ComSegDict"]
@@ -385,15 +379,14 @@
         :param file_extension: file extension of the centroid dictionary
         :type file_extension: str
         :param centroid_csv_key: column name  of the centroid csv file
         :type centroid_csv_key: dict
         :return:
         """
 
-
         for img_name in tqdm(self):
 
             if path_cell_centroid is not None:
                 assert self.dataset.dict_centroid is None, "The dict_centroid attribute of the dataset is not None. Please remove it or set it to None."
                 if str(file_extension)[-4:] == ".npy":
                     dict_cell_centroid = np.load(Path(path_cell_centroid) / (img_name + file_extension), allow_pickle=True).item()
                 elif str(file_extension)[-4:] == ".csv":
```

### Comparing `comseg-0.0.8/src/comseg/model.py` & `comseg-0.1/src/comseg/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 labeled community with the clustering classes
 add centroid from the dataset in the graph
 apply dikstra to compute the distance between the centroid and the other nodes
 return a count matrix of the image
 """
 
 
-import alphashape
 
 #%%
 
 from tqdm import tqdm
 import networkx as nx
 import scipy.sparse as sp
 
 from sklearn.neighbors import NearestNeighbors
 from scipy.sparse import csr_matrix
 import anndata as ad
 import pandas as pd
-
-
+import alphashape
 
 import networkx.algorithms.community as nx_comm
 import numpy as np
 from sklearn.utils.extmath import weighted_mode
 from scipy.spatial import ConvexHull, Delaunay
 from .utils import custom_louvain ## for dev mode
 
@@ -809,14 +807,15 @@
         anndata.uns["df_spots"] = df_spots
         self.final_anndata = anndata
 
         if not return_polygon:
             return anndata, {}
         assert min_rna_per_cell > 0, "min_rna_per_cell should be > 0"
 
+
         list_polygon = []
         dict_polygon = {}
         for cell_index in range(len(list_cell_id)):
             csv_list_y = []
             csv_list_x = []
             if len(list_genes_name[cell_index]) >= min_rna_per_cell:
                 csv_list_y += list(np.array(list_cell_genes_coordinate[cell_index])[:, 1])
```

### Comparing `comseg-0.0.8/src/comseg/utils/custom_louvain.py` & `comseg-0.1/src/comseg/utils/custom_louvain.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/src/comseg/utils/plot.py` & `comseg-0.1/src/comseg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/src/comseg/utils/preprocessing.py` & `comseg-0.1/src/comseg/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `comseg-0.0.8/src/comseg/utils/utils_graph.py` & `comseg-0.1/src/comseg/utils/utils_graph.py`

 * *Files identical despite different names*

