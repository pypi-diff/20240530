# Comparing `tmp/galaxy-datasets-0.0.7.tar.gz` & `tmp/galaxy-datasets-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galaxy-datasets-0.0.7.tar", last modified: Wed Feb 22 14:27:50 2023, max compression
+gzip compressed data, was "dist/galaxy-datasets-0.0.8.tar", last modified: Thu Mar  2 22:02:27 2023, max compression
```

## Comparing `galaxy-datasets-0.0.7.tar` & `galaxy-datasets-0.0.8.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/check_internal_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/pytorch/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/pytorch/galaxy_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/pytorch/galaxy_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/demo_rings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/desi_low_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_candels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_decals_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_desi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_rings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/label_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/tidal.py
--rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/shared/torchvision_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/tensorflow/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/galaxy_datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/galaxy_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 14:27:50.000000 galaxy-datasets-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-22 14:27:41.000000 galaxy-datasets-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/check_internal_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/pytorch/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/pytorch/galaxy_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/pytorch/galaxy_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/demo_gz_candels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/demo_rings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/desi_low_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_candels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_decals_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_desi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_hubble_euclidized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_rings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/label_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/tidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14703 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/shared/torchvision_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/tensorflow/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/galaxy_datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/galaxy_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 22:02:27.000000 galaxy-datasets-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-02 22:02:15.000000 galaxy-datasets-0.0.8/setup.py
```

### Comparing `galaxy-datasets-0.0.7/LICENSE` & `galaxy-datasets-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/PKG-INFO` & `galaxy-datasets-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-datasets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Galaxy Zoo datasets for PyTorch/TensorFlow
 Home-page: https://github.com/mwalmsley/galaxy-datasets
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -26,28 +26,29 @@
 
 You may also be interested in [Galaxy MNIST](https://github.com/mwalmsley/galaxy_mnist) as a simple dataset for teaching/debugging.
  
 
 | Name      | Method | PyTorch Dataset | Published | Downloadable | Galaxies
 | ----------- | ----- | ----------- | --- | ---- | ---- |
 | Galaxy Zoo 2 | gz2 | GZ2 | &#x2611; | &#x2611; | ~210k (main sample) |
-| GZ Hubble   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
+| GZ Hubble*   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
 | GZ CANDELS   | gz_candels | GZCandels | &#x2611; | &#x2611; | ~50k |
 | GZ DECaLS GZD-5 | gz_decals_5 | GZDecals5 | &#x2611; | &#x2611; | ~230k (GZD-5 only)|
 | GZ Rings | gz_rings | GZRings | &#x2612; | &#x2611; | ~93k |
-| GZ DESI  | gz_desi | GZDesi | &#x2612; | z < 0.1 only | ~375k + 8.3m unlabelled |
+| GZ DESI  | gz_desi | GZDesi | &#x2612; | WIP | WIP |
 | CFHT Tidal* | tidal | Tidal | &#x2611; | &#x2611; | 1760 (expert) |
 
 Any datasets marked as downloadable but not marked as published are only downloadable internally (for development purposes).
 
 For each dataset, you must cite/acknowledge the GZ data release paper and the original telescope survey from which the images were derived. See [data.galaxyzoo.org](data.galaxyzoo.org) for the data release paper citations to use.
 
-*CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
-MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232).
-We include it here as a challenging fine-grained morphology classification task with little labelled data.
+*GZ Hubble is also available in "euclidised" form (i.e. with the Euclid PSF applied) to Euclid collaboration members. The method is `gz_hubble_euclidised`. Courtesy of Ben Aussel.
+
+**CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
+MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232). We include it here as a challenging fine-grained morphology classification task with little labelled data.
 
 ## Installation
 
 Installing [zoobot](www.github/mwalmsley/zoobot) will automatically install this package as a dependency.
 
 To install directly:
```

### Comparing `galaxy-datasets-0.0.7/README.md` & `galaxy-datasets-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 
 You may also be interested in [Galaxy MNIST](https://github.com/mwalmsley/galaxy_mnist) as a simple dataset for teaching/debugging.
  
 
 | Name      | Method | PyTorch Dataset | Published | Downloadable | Galaxies
 | ----------- | ----- | ----------- | --- | ---- | ---- |
 | Galaxy Zoo 2 | gz2 | GZ2 | &#x2611; | &#x2611; | ~210k (main sample) |
-| GZ Hubble   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
+| GZ Hubble*   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
 | GZ CANDELS   | gz_candels | GZCandels | &#x2611; | &#x2611; | ~50k |
 | GZ DECaLS GZD-5 | gz_decals_5 | GZDecals5 | &#x2611; | &#x2611; | ~230k (GZD-5 only)|
 | GZ Rings | gz_rings | GZRings | &#x2612; | &#x2611; | ~93k |
-| GZ DESI  | gz_desi | GZDesi | &#x2612; | z < 0.1 only | ~375k + 8.3m unlabelled |
+| GZ DESI  | gz_desi | GZDesi | &#x2612; | WIP | WIP |
 | CFHT Tidal* | tidal | Tidal | &#x2611; | &#x2611; | 1760 (expert) |
 
 Any datasets marked as downloadable but not marked as published are only downloadable internally (for development purposes).
 
 For each dataset, you must cite/acknowledge the GZ data release paper and the original telescope survey from which the images were derived. See [data.galaxyzoo.org](data.galaxyzoo.org) for the data release paper citations to use.
 
-*CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
-MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232).
-We include it here as a challenging fine-grained morphology classification task with little labelled data.
+*GZ Hubble is also available in "euclidised" form (i.e. with the Euclid PSF applied) to Euclid collaboration members. The method is `gz_hubble_euclidised`. Courtesy of Ben Aussel.
+
+**CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
+MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232). We include it here as a challenging fine-grained morphology classification task with little labelled data.
 
 ## Installation
 
 Installing [zoobot](www.github/mwalmsley/zoobot) will automatically install this package as a dependency.
 
 To install directly:
```

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/__init__.py` & `galaxy-datasets-0.0.8/galaxy_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/pytorch/datasets.py` & `galaxy-datasets-0.0.8/galaxy_datasets/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/pytorch/galaxy_datamodule.py` & `galaxy-datasets-0.0.8/galaxy_datasets/pytorch/galaxy_datamodule.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/pytorch/galaxy_dataset.py` & `galaxy-datasets-0.0.8/galaxy_datasets/pytorch/galaxy_dataset.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/__init__.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/demo_rings.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/demo_rings.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from galaxy_datasets.shared import download_utils
 
 
 def demo_rings(root, train, download):
     logging.info('Setting up demo_rings dataset')
     resources = [
-        ('https://dl.dropboxusercontent.com/s/qwf4irf0xzj96sm/demo_rings_train_catalog.parquet', 'cf650961bcdd889f201ed049fb825085'),  # train catalog
-        ('https://dl.dropboxusercontent.com/s/b0w3ffoww4t9bq0/demo_rings_test_catalog.parquet', 'e84d19d279a02fb3a319d4e8aff4d724'),  # test catalog
-        ('https://dl.dropboxusercontent.com/s/54016cw50ide3y8/demo_rings_images.tar.xz', '36a75712ce1929b0c376ba3a8d51b7a8')  # the images
+        ('https://dl.dropboxusercontent.com/s/4cfb9xbnlkvbkv1/demo_rings_train_catalog.parquet', '6b3ff71b8893175cbdb9dc092ed0dbd9'),  # train catalog
+        ('https://dl.dropboxusercontent.com/s/xghqujm41ujjlko/demo_rings_test_catalog.parquet', 'e63e13b57e8dbe55c1cf339dee5395ae'),  # test catalog
+        ('https://dl.dropboxusercontent.com/s/80s5j6dygtw0gu6/demo_rings_images.tar.gz', 'b8489af55d54b6965d4b037a4f952f3c')  # the images
     ]
     images_to_spotcheck = [
-        'images/J000411.19+020924.0.jpg',
-        'images/J235601.89+073123.0.jpg'
+        'images/313982/313982_3559.jpg',
+        'images/374032/374032_255.jpg'
     ]
 
     downloader = download_utils.DatasetDownloader(root, resources, images_to_spotcheck)
     if download is True:
         downloader.download()
 
     if train:
@@ -37,8 +37,8 @@
     return catalog, label_cols
 
 
 if __name__ == '__main__':
 
     logging.basicConfig(level=logging.INFO)
     
-    demo_rings(root='/home/walml/repos/galaxy-datasets/roots/demo_rings', train=True, download=True)
+    demo_rings(root='/Users/user/repos/galaxy-datasets/roots/demo_rings', train=True, download=True)
```

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/desi_low_z.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/desi_low_z.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/download_utils.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/download_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz2.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz2.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_candels.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_rings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,47 @@
-
 import os
 import logging
 
 import pandas as pd
 
 from galaxy_datasets.shared import download_utils, label_metadata
+from galaxy_datasets.check_internal_urls import INTERNAL_URLS_EXIST
+if not INTERNAL_URLS_EXIST:
+    raise FileNotFoundError
+from galaxy_datasets.shared import internal_urls
 
 
-def gz_candels(root, train, download):
-    logging.info('Setting up gz_candels dataset')
+def gz_rings(root, train, download):
+    logging.info('Setting up gz_rings dataset')
     resources = [
-        ('https://dl.dropboxusercontent.com/s/cnjvdinnhh1r1md/candels_ortho_train_catalog.parquet', '90593d1bab79a608cf0e645d6fd8e741'),  # train catalog
-        ('https://dl.dropboxusercontent.com/s/y83v1gktw72hs0f/candels_ortho_test_catalog.parquet', '1062993dd8df09684b335678ab3fa8e3'),  # test catalog
-        ('https://dl.dropboxusercontent.com/s/d67we9xsn8vyr5k/candels_images.tar.gz', 'b621ee4e650cf084a1a0c1fe5c9d0a21')  # the images
+        (internal_urls.rings_train_catalog, 'e2fb6b2bca45cd7f1c58f5b4089a5976'),  # train catalog
+        (internal_urls.rings_test_catalog, '6e3f362a6e19ecd02675eaa48f6727f0'),  # test catalog
+        (internal_urls.rings_images, 'd0950250436a05ce88de747e6af825b6')  # the images
     ]
-    images_to_spotcheck = ['COS_9933.jpg', 'UDS_21986.jpg', 'GDS_9405.jpg']
+    images_to_spotcheck = []
 
     downloader = download_utils.DatasetDownloader(root, resources, images_to_spotcheck)
     if download is True:
         downloader.download()
 
-    # label_cols = [question + answer for question, answers in candels_ortho_pairs.items() for answer in answers]  # defined below, globally in this script (for imports elsewhere)
-    label_cols = label_metadata.candels_ortho_label_cols  # see below
-
-    useful_columns = label_cols + ['filename']
+    # useful_columns = label_cols + ['subfolder', 'filename']
+    useful_columns = None
     if train:
-        train_catalog_loc = os.path.join(root, 'candels_ortho_train_catalog.parquet')
+        train_catalog_loc = os.path.join(root, 'rings_train_catalog.parquet')
         catalog = pd.read_parquet(train_catalog_loc, columns=useful_columns)
     else:
-        test_catalog_loc = os.path.join(root, 'candels_ortho_test_catalog.parquet')
+        test_catalog_loc = os.path.join(root, 'rings_test_catalog.parquet')
         catalog = pd.read_parquet(test_catalog_loc, columns=useful_columns)
 
-    catalog['file_loc'] = catalog.apply(lambda x: os.path.join(downloader.image_dir, x['filename']), axis=1)  # no subfolder
+    catalog['file_loc'] = catalog.apply(lambda x: os.path.join(downloader.image_dir, x['subfolder'], x['filename']), axis=1)
+
+    label_cols = label_metadata.rings_label_cols
 
-    logging.info('gz_candels dataset ready')
+    logging.info('gz_rings dataset ready')
     return catalog, label_cols
+
+
+if __name__ == '__main__':
+
+    logging.basicConfig(level=logging.INFO)
+    
+    gz_rings(root='/Users/user/repos/galaxy-datasets/roots/gz_rings', train=True, download=True)
```

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_decals_5.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_decals_5.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_desi.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_desi.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_hubble.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_hubble.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/gz_rings.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/gz_hubble_euclidized.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 import os
 import logging
 
 import pandas as pd
 
+from zoobot.shared import label_metadata
+
 from galaxy_datasets.shared import download_utils, label_metadata
 from galaxy_datasets.check_internal_urls import INTERNAL_URLS_EXIST
 if not INTERNAL_URLS_EXIST:
     raise FileNotFoundError
 from galaxy_datasets.shared import internal_urls
 
 
-def gz_rings(root, train, download):
-    logging.info('Setting up gz_rings dataset')
+def gz_hubble_euclidized(root, train, download):
+    logging.info('Setting up gz_hubble_euclidized dataset')
     resources = [
-        (internal_urls.rings_train_catalog, 'e2fb6b2bca45cd7f1c58f5b4089a5976'),  # train catalog
-        (internal_urls.rings_test_catalog, '6e3f362a6e19ecd02675eaa48f6727f0'),  # test catalog
-        (internal_urls.rings_images, 'd0950250436a05ce88de747e6af825b6')  # the images
+        (internal_urls.hubble_euclidised_train_catalog, '99a92bb1abd47966f77a7b04e4e310ac'),  # train catalog
+        (internal_urls.hubble_euclidised_test_catalog, '4f628f5e7d3282fbfa7ed4b0d7d91b11'),  # test catalog
+        (internal_urls.hubble_euclidised_images, 'baee3a003631be238bb9cd6650cf03bf')
     ]
-    images_to_spotcheck = []
+    images_to_spotcheck = ['20000011.jpg', '20164189.jpg', '203191082.jpg']
 
     downloader = download_utils.DatasetDownloader(root, resources, images_to_spotcheck)
     if download is True:
         downloader.download()
 
-    # useful_columns = label_cols + ['subfolder', 'filename']
-    useful_columns = None
+    label_cols = label_metadata.hubble_ortho_label_cols
+
+    useful_columns = label_cols + ['filename']
     if train:
-        train_catalog_loc = os.path.join(root, 'rings_train_catalog.parquet')
+        train_catalog_loc = os.path.join(root, 'catalog_euclid_train.parquet')
         catalog = pd.read_parquet(train_catalog_loc, columns=useful_columns)
     else:
-        test_catalog_loc = os.path.join(root, 'rings_test_catalog.parquet')
+        test_catalog_loc = os.path.join(root, 'catalog_euclid_test.parquet')
         catalog = pd.read_parquet(test_catalog_loc, columns=useful_columns)
 
-    catalog['file_loc'] = catalog.apply(lambda x: os.path.join(downloader.image_dir, x['subfolder'], x['filename']), axis=1)
-
-    label_cols = label_metadata.rings_label_cols
+    catalog['file_loc'] = catalog.apply(lambda x: os.path.join(downloader.image_dir, x['filename']), axis=1)  # no subfolder
 
-    logging.info('gz_rings dataset ready')
+    logging.info('gz_hubble_euclidized dataset ready')
     return catalog, label_cols
 
+
+if __name__ == '__main__':
+
+
+    gz_hubble_euclidized(
+        root='/nvme1/scratch/walml/repos/galaxy-datasets/roots/gz_hubble_euclidised',
+        train=True,
+        download=True
+        )
```

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/label_metadata.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/label_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/tidal.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/tidal.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/shared/torchvision_utils.py` & `galaxy-datasets-0.0.8/galaxy_datasets/shared/torchvision_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/tensorflow/datasets.py` & `galaxy-datasets-0.0.8/galaxy_datasets/tensorflow/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets/transforms.py` & `galaxy-datasets-0.0.8/galaxy_datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets.egg-info/PKG-INFO` & `galaxy-datasets-0.0.8/galaxy_datasets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-datasets
-Version: 0.0.7
+Version: 0.0.8
 Summary: Galaxy Zoo datasets for PyTorch/TensorFlow
 Home-page: https://github.com/mwalmsley/galaxy-datasets
 Author: Mike Walmsley
 Author-email: walmsleymk1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
@@ -26,28 +26,29 @@
 
 You may also be interested in [Galaxy MNIST](https://github.com/mwalmsley/galaxy_mnist) as a simple dataset for teaching/debugging.
  
 
 | Name      | Method | PyTorch Dataset | Published | Downloadable | Galaxies
 | ----------- | ----- | ----------- | --- | ---- | ---- |
 | Galaxy Zoo 2 | gz2 | GZ2 | &#x2611; | &#x2611; | ~210k (main sample) |
-| GZ Hubble   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
+| GZ Hubble*   | gz_hubble | GZHubble | &#x2611; | &#x2611; | ~106k (main sample) |
 | GZ CANDELS   | gz_candels | GZCandels | &#x2611; | &#x2611; | ~50k |
 | GZ DECaLS GZD-5 | gz_decals_5 | GZDecals5 | &#x2611; | &#x2611; | ~230k (GZD-5 only)|
 | GZ Rings | gz_rings | GZRings | &#x2612; | &#x2611; | ~93k |
-| GZ DESI  | gz_desi | GZDesi | &#x2612; | z < 0.1 only | ~375k + 8.3m unlabelled |
+| GZ DESI  | gz_desi | GZDesi | &#x2612; | WIP | WIP |
 | CFHT Tidal* | tidal | Tidal | &#x2611; | &#x2611; | 1760 (expert) |
 
 Any datasets marked as downloadable but not marked as published are only downloadable internally (for development purposes).
 
 For each dataset, you must cite/acknowledge the GZ data release paper and the original telescope survey from which the images were derived. See [data.galaxyzoo.org](data.galaxyzoo.org) for the data release paper citations to use.
 
-*CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
-MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232).
-We include it here as a challenging fine-grained morphology classification task with little labelled data.
+*GZ Hubble is also available in "euclidised" form (i.e. with the Euclid PSF applied) to Euclid collaboration members. The method is `gz_hubble_euclidised`. Courtesy of Ben Aussel.
+
+**CFHT Tidal is not a Galaxy Zoo dataset, but rather a small expert-labelled dataset of tidal features from [Atkinson 2013](https://doi.org/10.1088/0004-637X/765/1/28).
+MW reproduced and modified the images in [Walmsley 2019](https://doi.org/10.1093/mnras/sty3232). We include it here as a challenging fine-grained morphology classification task with little labelled data.
 
 ## Installation
 
 Installing [zoobot](www.github/mwalmsley/zoobot) will automatically install this package as a dependency.
 
 To install directly:
```

### Comparing `galaxy-datasets-0.0.7/galaxy_datasets.egg-info/SOURCES.txt` & `galaxy-datasets-0.0.8/galaxy_datasets.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 galaxy_datasets.egg-info/requires.txt
 galaxy_datasets.egg-info/top_level.txt
 galaxy_datasets/pytorch/__init__.py
 galaxy_datasets/pytorch/datasets.py
 galaxy_datasets/pytorch/galaxy_datamodule.py
 galaxy_datasets/pytorch/galaxy_dataset.py
 galaxy_datasets/shared/__init__.py
+galaxy_datasets/shared/demo_gz_candels.py
 galaxy_datasets/shared/demo_rings.py
 galaxy_datasets/shared/desi_low_z.py
 galaxy_datasets/shared/download_utils.py
 galaxy_datasets/shared/gz2.py
 galaxy_datasets/shared/gz_candels.py
 galaxy_datasets/shared/gz_decals_5.py
 galaxy_datasets/shared/gz_desi.py
 galaxy_datasets/shared/gz_hubble.py
+galaxy_datasets/shared/gz_hubble_euclidized.py
 galaxy_datasets/shared/gz_rings.py
 galaxy_datasets/shared/label_metadata.py
 galaxy_datasets/shared/tidal.py
 galaxy_datasets/shared/torchvision_utils.py
 galaxy_datasets/tensorflow/__init__.py
 galaxy_datasets/tensorflow/datasets.py
```

### Comparing `galaxy-datasets-0.0.7/setup.py` & `galaxy-datasets-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="galaxy-datasets",
-    version="0.0.7",
+    version="0.0.8",
     author="Mike Walmsley",
     author_email="walmsleymk1@gmail.com",
     description="Galaxy Zoo datasets for PyTorch/TensorFlow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mwalmsley/galaxy-datasets",
     classifiers=[
```

