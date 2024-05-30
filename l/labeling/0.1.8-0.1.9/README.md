# Comparing `tmp/labeling-0.1.8.tar.gz` & `tmp/labeling-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeling-0.1.8.tar", last modified: Thu Mar 31 08:45:45 2022, max compression
+gzip compressed data, was "labeling-0.1.9.tar", last modified: Wed Apr 13 09:49:42 2022, max compression
```

## Comparing `labeling-0.1.8.tar` & `labeling-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-03-31 08:45:45.222480 labeling-0.1.8/
--rw-rw-rw-   0        0        0     1341 2022-03-29 14:41:50.000000 labeling-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1837 2022-03-31 08:45:45.220446 labeling-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1098 2021-06-24 11:57:38.000000 labeling-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-03-31 08:45:45.198464 labeling-0.1.8/labeling/
--rw-rw-rw-   0        0        0     9773 2022-03-31 08:27:35.000000 labeling-0.1.8/labeling/Labeling.py
--rw-rw-rw-   0        0        0       90 2022-03-28 14:42:13.000000 labeling-0.1.8/labeling/__init__.py
--rw-rw-rw-   0        0        0     4050 2022-03-30 20:47:35.000000 labeling-0.1.8/labeling/bsoncontainer.py
-drwxrwxrwx   0        0        0        0 2022-03-31 08:45:45.216479 labeling-0.1.8/labeling.egg-info/
--rw-rw-rw-   0        0        0     1837 2022-03-31 08:45:43.000000 labeling-0.1.8/labeling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2022-03-31 08:45:45.000000 labeling-0.1.8/labeling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-31 08:45:43.000000 labeling-0.1.8/labeling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-03-31 08:45:44.000000 labeling-0.1.8/labeling.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-03-31 08:45:44.000000 labeling-0.1.8/labeling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      203 2022-01-13 14:57:05.000000 labeling-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-03-31 08:45:45.223447 labeling-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1101 2022-03-31 08:32:17.000000 labeling-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-04-13 09:49:42.622557 labeling-0.1.9/
+-rw-rw-rw-   0        0        0     1341 2022-03-29 14:41:50.000000 labeling-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1837 2022-04-13 09:49:42.622557 labeling-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1098 2021-06-24 11:57:38.000000 labeling-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2022-04-13 09:49:42.612556 labeling-0.1.9/labeling/
+-rw-rw-rw-   0        0        0     9511 2022-04-12 13:38:43.000000 labeling-0.1.9/labeling/Labeling.py
+-rw-rw-rw-   0        0        0     3787 2022-04-06 12:32:44.000000 labeling-0.1.9/labeling/LabelingData.py
+-rw-rw-rw-   0        0        0       88 2022-04-06 11:54:33.000000 labeling-0.1.9/labeling/__init__.py
+drwxrwxrwx   0        0        0        0 2022-04-13 09:49:42.620558 labeling-0.1.9/labeling.egg-info/
+-rw-rw-rw-   0        0        0     1837 2022-04-13 09:49:42.000000 labeling-0.1.9/labeling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2022-04-13 09:49:42.000000 labeling-0.1.9/labeling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-13 09:49:42.000000 labeling-0.1.9/labeling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2022-04-13 09:49:42.000000 labeling-0.1.9/labeling.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-04-13 09:49:42.000000 labeling-0.1.9/labeling.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      179 2022-04-06 12:20:50.000000 labeling-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-04-13 09:49:42.622557 labeling-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2022-04-13 09:41:21.000000 labeling-0.1.9/setup.py
```

### Comparing `labeling-0.1.8/LICENSE` & `labeling-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `labeling-0.1.8/PKG-INFO` & `labeling-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeling
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to create labeling/segmentation information based on pixel values.
 Home-page: https://github.com/Labelings/pyLabeling
 Author: Tom Burke
 Author-email: burke@mpi-cbg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Labelings/pyLabeling/issues
 Platform: UNKNOWN
```

### Comparing `labeling-0.1.8/README.md` & `labeling-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `labeling-0.1.8/labeling/Labeling.py` & `labeling-0.1.9/labeling/Labeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import List, Callable, Tuple, T, Dict
 
 import numpy as np
 from PIL import Image
 from tifffile import imread
 
-import labeling.bsoncontainer as bc
+from .LabelingData import LabelingData
 
 
 class LabelSet:
     set: set()
     source: str()
 
     def __init__(self, source="", element=None):
@@ -36,15 +36,15 @@
         self.__segmentation_source = {}
         self.metadata = None
         self.__img_filename = None
 
     @classmethod
     def from_file(cls, path: str):
         labeling = cls.__new__(cls)
-        container = bc.BsonContainer.decode(path)
+        container = LabelingData.decode(path)
         labeling.result_image = container.get_image()
         labeling.__image_resolution = labeling.result_image.shape
         labeling.label_sets = container.labelSets
         labeling.metadata = container.metadata
         labeling.__img_filename = os.path.split(path)[1].replace(".labeling.bson", ".tif")
         labeling.__segmentation_source = dict.fromkeys(range(container.numSources), range(container.numSources))
         return labeling
@@ -65,25 +65,26 @@
         labeling = Labeling()
         labeling.__list_of_unique_ids = np.unique(first_image)
         labeling.__image_resolution = first_image.shape
         labeling.result_image = np.zeros(first_image.shape, first_image.dtype)
         labeling.add_image(first_image, source_id)
         return labeling
 
-    def iterate_over_images(self, images: List[np.ndarray], source_ids=None) ->  List[Dict[str, LabelSet]]:
+    def iterate_over_images(self, images: List[np.ndarray], source_ids=None) -> List[Dict[str, LabelSet]]:
         # iterate over all images
         ret = []
         for image, source_id in zip(images, source_ids):
             ret.append(self.add_image(image, source_id))
         return ret
 
     def add_image(self, image: np.ndarray, source_id=None) -> Dict[str, LabelSet]:
         return self.add_segments(image, (0, 0), source_id=source_id)
 
-    def add_segments(self, patch: np.ndarray, position: Tuple, merge: dict = None, source_id=None) -> Dict[str, LabelSet]:
+    def add_segments(self, patch: np.ndarray, position: Tuple, merge: dict = None, source_id=None) -> Dict[
+        str, LabelSet]:
         list_of_unique_labelvalues = set()
         segment_mapping = {}
         __unique_map_id_id_label = {}
         temp = np.reshape(self.result_image, self.__image_resolution)
         with np.nditer(patch, flags=["multi_index"], op_flags=["readonly"]) as it:
             for val in it:
                 if val.item() != 0:
@@ -121,62 +122,56 @@
 
     def add_segmentation_source(self, source_id, __label_value) -> None:
         if source_id is not None:
             if str(source_id) not in self.__segmentation_source.keys():
                 self.__segmentation_source[str(source_id)] = set()
             self.__segmentation_source[str(source_id)].add(__label_value)
 
-    def save_result(self, path: str, cleanup: bool = False, save_json: bool = False):
+    def save_result(self, path: str, cleanup: bool = False):
         if cleanup:
             self.__cleanup_labelsets()
         img = Image.fromarray(np.reshape(self.result_image, self.__image_resolution))
         path, filename = os.path.split(path)
         img.save(os.path.join(path, filename + '.tif'), 'tiff')
         self.__img_filename = filename + '.tif'
-        bson_con = bc.BsonContainer.fromValues(2, len(self.label_sets), len(self.__segmentation_source),
-                                               self.__img_filename, {},
-                                               {key:list(value) for (key,value) in self.label_sets.items()}, self.metadata)
-        bson_con.encode_and_save(os.path.join(path, filename + '.labeling.bson'))
-        # optional, just to easily content check
-        if save_json:
-            bson_con.save_as_json(os.path.join(path, filename + '.json'))
-        return np.reshape(self.result_image, self.__image_resolution), bson_con
+        label_data = LabelingData.fromValues(2, len(self.label_sets), len(self.__segmentation_source),
+                                             self.__img_filename, {},
+                                             {key: list(value) for (key, value) in
+                                              self.label_sets.items()}, self.metadata)
+        label_data.save_as_json(os.path.join(path, filename + '.lbl.json'))
+        return np.reshape(self.result_image, self.__image_resolution), label_data
 
-    def get_result(self, cleanup: bool = False) -> (np.array, bc.BsonContainer):
+    def get_result(self, cleanup: bool = False) -> (np.array, LabelingData):
         if cleanup:
             self.__cleanup_labelsets()
         return np.reshape(self.result_image, self.__image_resolution), \
-               bc.BsonContainer.fromValues(2,
-                                           len(self.label_sets),
-                                           len(self.__segmentation_source),
-                                           self.__img_filename, {},
-                                           {key:list(value) for (key,value) in self.label_sets.items()},
-                                           self.metadata)
+               LabelingData.fromValues(2,
+                                       len(self.label_sets),
+                                       len(self.__segmentation_source),
+                                       self.__img_filename, {},
+                                       {key: list(value) for (key, value) in self.label_sets.items()},
+                                       self.metadata)
 
     def __cleanup_labelsets(self) -> None:
         # cleanup labelSets
         _, idx = np.unique(self.result_image, return_index=True)
         t = list(self.result_image[np.sort(idx)])
         if 0 not in t:
-            t.insert(0,0)
+            t.insert(0, 0)
         relabels = range(len(t) + 1)
 
         temp = np.zeros(self.result_image.shape, np.int8)
         for a, b in zip(t, relabels):
             temp[self.result_image == a] = b
         self.result_image = temp
         lookup_table = dict(zip([str(i) for i in t], relabels))
-        print(t)
-        print(lookup_table)
         # reconstruct the labelsets
         new_label_sets = {}
         segments = self.__segment_fragment_mapping().keys()
-        print(self.label_sets)
-        segment_remapping = dict(zip(segments, range(1, len(segments)+2)))
-        print(segment_remapping)
+        segment_remapping = dict(zip(segments, range(1, len(segments) + 2)))
         for setname, labelset in self.label_sets.items():
             if setname in lookup_table.keys():
                 new_label_sets[str(lookup_table[setname])] = [segment_remapping[x] for x in list(labelset)]
         for key, value in self.__segmentation_source.items():
             self.__segmentation_source[key] = list(value)
         self.label_sets = new_label_sets
```

### Comparing `labeling-0.1.8/labeling/bsoncontainer.py` & `labeling-0.1.9/labeling/LabelingData.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,93 @@
 import json
 import os
 from typing import Callable, T
 
-import bson
 from tifffile import imread
 
 
-class BsonContainer(dict):
+class LabelingData(dict):
 
     def __init__(self):
         self.version = 2
         self.numSets = 0
         self.numSources = 0
         self.indexImg = ""
-        self.labelMapping = {}
+        self.labelMapping = None
         self.labelSets = {}
-        self.metadata = {}
+        self.metadata = None
 
     @classmethod
     def fromValues(cls, version: int = 2, num_sets: int = 0, num_sources: int = 0, index_img: str = "",
-                   label_mapping: dict = {},
+                   label_mapping: dict = None,
                    label_sets: dict = {}, metadata: dict() = None):
-        obj = BsonContainer()
+        obj = LabelingData()
         obj.numSets = num_sets
         obj.numSources = num_sources
         obj.indexImg = index_img
-        obj.labelMapping = label_mapping
+        if label_mapping is not None:
+            obj.labelMapping = label_mapping
         obj.labelSets = label_sets
         obj.version = version
         if metadata is not None:
             obj.metadata = metadata
         return obj
 
     @classmethod
     def fromDict(cls, data: dict):
-        obj = BsonContainer()
+        obj = LabelingData()
         obj.version = data["version"]
         obj.numSets = data["numSets"]
         obj.numSources = data["numSources"]
         obj.indexImg = data["indexImg"]
         obj.labelMapping = data["labelMapping"]
         obj.labelSets = data["labelSets"]
         obj.metadata = data["metadata"]
         return obj
 
-    def encode(self):
-        return bson.encode(vars(self))
-
-    def encode_and_save(self, path: str):
-        data = bson.encode(vars(self))
-        with open(path, 'wb+') as f:
-            f.write(data)
-
     def encodewithfunc(self, path: str, func: Callable[[T], int]):
         for labelset in self.labelSets.values():
             i = 0
             for label in labelset:
                 t = func(label)
                 labelset[i] = t
                 i += 1
 
-        data = bson.encode(vars(self))
-        with open(path, 'wb+') as f:
-            f.write(data)
+        self.save_as_json(path)
 
     def save_as_json(self, path: str):
         with open(path, 'w') as outfile:
             json.dump(vars(self), outfile)
 
     @staticmethod
     def decode(path: str):
         with open(path, 'rb') as f:
-            data = bson.decode(f.read())
+            data = json.load(f.read())
             data["indexImg"] = os.path.join(os.path.dirname(os.path.realpath(f.name)), data["indexImg"])
             if "metadata" not in data.keys():
-                return BsonContainer.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
+                return LabelingData.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
                                                 data["labelMapping"],
                                                 data["labelSets"])
-            return BsonContainer.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
+            return LabelingData.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
                                             data["labelMapping"], data["labelSets"], data["metadata"])
 
     @staticmethod
     def decode_withfunc(path, func: Callable[[int], T]):
-        with open(path, 'rb') as f:
-            data = bson.decode(f.read())
+        with open(path, 'r') as f:
+            data = json.load(f.read())
             transformed_labelsets = {}
             for key, labelset in data['labelSets'].items():
                 transformed_labelsets[key] = set()
                 for label in labelset:
                     transformed_labelsets[key].add(func(label))
 
             if "metadata" not in data.keys():
-                return BsonContainer.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
+                return LabelingData.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
                                                 data["labelMapping"], data["labelSets"])
-            return BsonContainer.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
+            return LabelingData.fromValues(data["version"], data["numSets"], data["numSources"], data["indexImg"],
                                             data["labelMapping"], data["labelSets"], data["metadata"])
 
     def get_image(self):
         return imread(self.indexImg)
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
```

### Comparing `labeling-0.1.8/labeling.egg-info/PKG-INFO` & `labeling-0.1.9/labeling.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeling
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to create labeling/segmentation information based on pixel values.
 Home-page: https://github.com/Labelings/pyLabeling
 Author: Tom Burke
 Author-email: burke@mpi-cbg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Labelings/pyLabeling/issues
 Platform: UNKNOWN
```

### Comparing `labeling-0.1.8/setup.py` & `labeling-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="labeling",
-    version="0.1.8",
+    version="0.1.9",
     author="Tom Burke",
     author_email="burke@mpi-cbg.de",
     description="A package to create labeling/segmentation information based on pixel values.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Labelings/pyLabeling",
     project_urls={
@@ -22,13 +22,12 @@
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent"
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=[
-        "pymongo==3.11.0",
         "tifffile==2021.4.8",
         "pillow==9.0.1",
         "numpy==1.21"
     ],
 )
```

