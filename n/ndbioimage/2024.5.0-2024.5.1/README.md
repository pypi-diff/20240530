# Comparing `tmp/ndbioimage-2024.5.0.tar.gz` & `tmp/ndbioimage-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.5.0.tar", max compression
+gzip compressed data, was "ndbioimage-2024.5.1.tar", max compression
```

## Comparing `ndbioimage-2024.5.0.tar` & `ndbioimage-2024.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.5.0/LICENSE
--rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.5.0/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.5.0/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    54670 2024-05-13 09:41:04.263451 ndbioimage-2024.5.0/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.5.0/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.5.0/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.5.0/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28254 2024-04-29 11:09:41.232812 ndbioimage-2024.5.0/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.5.0/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.5.0/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.5.0/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.5.0/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.5.0/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.5.0/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1248 2024-05-13 09:41:04.375452 ndbioimage-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.5.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.5.1/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54740 2024-05-30 08:48:33.971792 ndbioimage-2024.5.1/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-30 08:48:34.027792 ndbioimage-2024.5.1/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.5.1/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     9017 2024-05-30 08:58:07.766055 ndbioimage-2024.5.1/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28254 2024-04-29 11:09:41.232812 ndbioimage-2024.5.1/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.5.1/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.5.1/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.5.1/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.5.1/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.5.1/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.5.1/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1248 2024-05-30 08:49:40.520054 ndbioimage-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.5.1/PKG-INFO
```

### Comparing `ndbioimage-2024.5.0/LICENSE` & `ndbioimage-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/README.md` & `ndbioimage-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/.DS_Store` & `ndbioimage-2024.5.1/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/__init__.py` & `ndbioimage-2024.5.1/ndbioimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import yaml
 from numpy.typing import ArrayLike, DTypeLike
 from ome_types import OME, from_xml, model, ureg
 from pint import set_application_registry
 from tiffwrite import IFD, IJTiffFile  # noqa
 from tqdm.auto import tqdm
 
-from .jvm import JVM
+from .jvm import JVM, JVMException
 from .transforms import Transform, Transforms
 
 try:
     __version__ = version(Path(__file__).parent.name)
 except Exception:  # noqa
     __version__ = 'unknown'
 
@@ -1130,20 +1130,21 @@
         if image.objective_settings:
             self.objective = find(instrument.objectives, id=image.objective_settings.id)
         else:
             self.objective = None
         try:
             t0 = find(image.pixels.planes, the_c=0, the_t=0, the_z=0).delta_t
             t1 = find(image.pixels.planes, the_c=0, the_t=self.shape['t'] - 1, the_z=0).delta_t
-            self.timeinterval = (t1 - t0) / (self.shape['t'] - 1) if self.shape['t'] > 1 else None
+            self.timeinterval = (t1 - t0) / (self.shape['t'] - 1) if self.shape['t'] > 1 and t1 > t0 else None
         except AttributeError:
             self.timeinterval = None
         try:
             self.binning = [int(i) for i in image.pixels.channels[0].detector_settings.binning.value.split('x')]
-            self.pxsize *= self.binning[0]
+            if self.pxsize is not None:
+                self.pxsize *= self.binning[0]
         except (AttributeError, IndexError, ValueError):
             self.binning = None
         self.channel_names = [channel.name for channel in image.pixels.channels]
         self.channel_names += [chr(97 + i) for i in range(len(self.channel_names), self.shape['c'])]
         self.cnamelist = self.channel_names
         try:
             optovars = [objective for objective in instrument.objectives if 'tubelens' in objective.id.lower()]
```

### Comparing `ndbioimage-2024.5.0/ndbioimage/jvm.py` & `ndbioimage-2024.5.1/ndbioimage/jvm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from pathlib import Path
 from urllib import request
 
+
+class JVMException(Exception):
+    pass
+
+
 try:
     class JVM:
         """ There can be only one java virtual machine per python process,
             so this is a singleton class to manage the jvm.
         """
         _instance = None
         vm_started = False
```

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/bfread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/bfread.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,88 +1,98 @@
 import multiprocessing
 from abc import ABC
 from multiprocessing import queues
-from traceback import print_exc
+from traceback import format_exc
+from pathlib import Path
 
 import numpy as np
 
-from .. import JVM, AbstractReader
+from .. import AbstractReader, JVM, JVMException
 
-jars = {'bioformats_package.jar':
-            'https://downloads.openmicroscopy.org/bio-formats/latest/artifacts/bioformats_package.jar'}
+jars = {'bioformats_package.jar': 'https://downloads.openmicroscopy.org/bio-formats/latest/artifacts/'
+                                  'bioformats_package.jar'}
 
 
 class JVMReader:
-    def __init__(self, path, series):
+    def __init__(self, path: Path, series: int) -> None:
         mp = multiprocessing.get_context('spawn')
         self.path = path
         self.series = series
         self.queue_in = mp.Queue()
         self.queue_out = mp.Queue()
-        self.queue_error = mp.Queue()
         self.done = mp.Event()
         self.process = mp.Process(target=self.run)
         self.process.start()
-        self.is_alive = True
+        status, message = self.queue_out.get()
+        if status == 'status' and message == 'started':
+            self.is_alive = True
+        else:
+            raise JVMException(message)
 
-    def close(self):
+    def close(self) -> None:
         if self.is_alive:
             self.done.set()
             while not self.queue_in.empty():
                 self.queue_in.get()
             self.queue_in.close()
             self.queue_in.join_thread()
             while not self.queue_out.empty():
                 print(self.queue_out.get())
             self.queue_out.close()
             self.process.join()
             self.process.close()
             self.is_alive = False
 
-    def frame(self, c, z, t):
+    def frame(self, c: int, z: int, t: int) -> np.ndarray:
         self.queue_in.put((c, z, t))
-        return self.queue_out.get()
+        status, message = self.queue_out.get()
+        if status == 'frame':
+            return message
+        else:
+            raise JVMException(message)
 
-    def run(self):
+    def run(self) -> None:
         """ Read planes from the image reader file.
             adapted from python-bioformats/bioformats/formatreader.py
         """
-        jvm = JVM(jars)
-        reader = jvm.image_reader()
-        ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
-        reader.setMetadataStore(ome_meta)
-        reader.setId(str(self.path))
-        reader.setSeries(self.series)
-
-        open_bytes_func = reader.openBytes
-        width, height = int(reader.getSizeX()), int(reader.getSizeY())
-
-        pixel_type = reader.getPixelType()
-        little_endian = reader.isLittleEndian()
-
-        if pixel_type == jvm.format_tools.INT8:
-            dtype = np.int8
-        elif pixel_type == jvm.format_tools.UINT8:
-            dtype = np.uint8
-        elif pixel_type == jvm.format_tools.UINT16:
-            dtype = '<u2' if little_endian else '>u2'
-        elif pixel_type == jvm.format_tools.INT16:
-            dtype = '<i2' if little_endian else '>i2'
-        elif pixel_type == jvm.format_tools.UINT32:
-            dtype = '<u4' if little_endian else '>u4'
-        elif pixel_type == jvm.format_tools.INT32:
-            dtype = '<i4' if little_endian else '>i4'
-        elif pixel_type == jvm.format_tools.FLOAT:
-            dtype = '<f4' if little_endian else '>f4'
-        elif pixel_type == jvm.format_tools.DOUBLE:
-            dtype = '<f8' if little_endian else '>f8'
-        else:
-            dtype = None
-
+        jvm = None
         try:
+            jvm = JVM(jars)
+            reader = jvm.image_reader()
+            ome_meta = jvm.metadata_tools.createOMEXMLMetadata()
+            reader.setMetadataStore(ome_meta)
+            reader.setId(str(self.path))
+            reader.setSeries(self.series)
+
+            open_bytes_func = reader.openBytes
+            width, height = int(reader.getSizeX()), int(reader.getSizeY())
+
+            pixel_type = reader.getPixelType()
+            little_endian = reader.isLittleEndian()
+
+            if pixel_type == jvm.format_tools.INT8:
+                dtype = np.int8
+            elif pixel_type == jvm.format_tools.UINT8:
+                dtype = np.uint8
+            elif pixel_type == jvm.format_tools.UINT16:
+                dtype = '<u2' if little_endian else '>u2'
+            elif pixel_type == jvm.format_tools.INT16:
+                dtype = '<i2' if little_endian else '>i2'
+            elif pixel_type == jvm.format_tools.UINT32:
+                dtype = '<u4' if little_endian else '>u4'
+            elif pixel_type == jvm.format_tools.INT32:
+                dtype = '<i4' if little_endian else '>i4'
+            elif pixel_type == jvm.format_tools.FLOAT:
+                dtype = '<f4' if little_endian else '>f4'
+            elif pixel_type == jvm.format_tools.DOUBLE:
+                dtype = '<f8' if little_endian else '>f8'
+            else:
+                dtype = None
+            self.queue_out.put(('status', 'started'))
+
             while not self.done.is_set():
                 try:
                     c, z, t = self.queue_in.get(True, 0.02)
                     if reader.isRGB() and reader.isInterleaved():
                         index = reader.getIndex(z, 0, t)
                         image = np.frombuffer(open_bytes_func(index), dtype)
                         image.shape = (height, width, reader.getSizeC())
@@ -147,27 +157,27 @@
                             image = lut[image, :]
                     else:
                         index = reader.getIndex(z, 0, t)
                         image = np.frombuffer(open_bytes_func(index), dtype)
                         image.shape = (height, width)
 
                     if image.ndim == 3:
-                        self.queue_out.put(image[..., c])
+                        self.queue_out.put(('frame', image[..., c]))
                     else:
-                        self.queue_out.put(image)
+                        self.queue_out.put(('frame', image))
                 except queues.Empty:  # noqa
                     continue
         except (Exception,):
-            print_exc()
-            self.queue_out.put(np.zeros((32, 32)))
+            self.queue_out.put(('error', format_exc()))
         finally:
-            jvm.kill_vm()
+            if jvm is not None:
+                jvm.kill_vm()
 
 
-def can_open(path):
+def can_open(path: Path) -> bool:
     try:
         jvm = JVM(jars)
         reader = jvm.image_reader()
         reader.getFormat(str(path))
         return True
     except (Exception,):
         return False
@@ -179,21 +189,20 @@
     """ This class is used as a last resort, when we don't have another way to open the file. We don't like it
         because it requires the java vm.
     """
     priority = 99  # panic and open with BioFormats
     do_not_pickle = 'reader', 'key', 'jvm'
 
     @staticmethod
-    def _can_open(path):
+    def _can_open(path: Path) -> bool:
         """ Use java BioFormats to make an ome metadata structure. """
         with multiprocessing.get_context('spawn').Pool(1) as pool:
-            ome = pool.map(can_open, (path,))[0]
-            return ome
+            return pool.map(can_open, (path,))[0]
 
-    def open(self):
+    def open(self) -> None:
         self.reader = JVMReader(self.path, self.series)
 
-    def __frame__(self, c, z, t):
+    def __frame__(self, c: int, z: int, t: int) -> np.ndarray:
         return self.reader.frame(c, z, t)
 
-    def close(self):
+    def close(self) -> None:
         self.reader.close()
```

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/cziread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/ndread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/seqread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/readers/tifread.py` & `ndbioimage-2024.5.1/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/ndbioimage/transforms.py` & `ndbioimage-2024.5.1/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.5.0/pyproject.toml` & `ndbioimage-2024.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.5.0"
+version = "2024.5.1"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.5.0/PKG-INFO` & `ndbioimage-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.10,<4.0
```

