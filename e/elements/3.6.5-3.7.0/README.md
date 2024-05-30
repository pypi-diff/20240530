# Comparing `tmp/elements-3.6.5.tar.gz` & `tmp/elements-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.6.5.tar", last modified: Wed May 29 13:31:49 2024, max compression
+gzip compressed data, was "elements-3.7.0.tar", last modified: Wed May 29 14:54:04 2024, max compression
```

## Comparing `elements-3.6.5.tar` & `elements-3.7.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.545950 elements-3.6.5/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.5/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.5/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 13:31:49.545950 elements-3.6.5/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.5/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-29 13:31:34.000000 elements-3.6.5/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.5/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 06:01:15.000000 elements-3.6.5/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.5/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.5/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.5/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.5/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.5/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    11869 2024-05-29 13:31:30.000000 elements-3.6.5/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.5/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.5/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.5/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.5/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.5/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.5/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.5/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.5/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.5/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-29 13:31:49.000000 elements-3.6.5/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.5/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.5/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-29 13:31:49.545950 elements-3.6.5/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.5/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 13:31:49.541950 elements-3.6.5/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.5/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.5/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.5/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1307 2024-05-22 06:01:09.000000 elements-3.6.5/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.5/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 14:54:04.377231 elements-3.7.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.7.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.7.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 14:54:04.377231 elements-3.7.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.7.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 14:54:04.373232 elements-3.7.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-29 14:53:36.000000 elements-3.7.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.7.0/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 06:01:15.000000 elements-3.7.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.7.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.7.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.7.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.7.0/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.7.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11957 2024-05-29 14:36:02.000000 elements-3.7.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.7.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.7.0/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.7.0/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.7.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.7.0/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.7.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.7.0/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.7.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.7.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 14:54:04.373232 elements-3.7.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-29 14:54:04.000000 elements-3.7.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-29 14:54:04.000000 elements-3.7.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-29 14:54:04.000000 elements-3.7.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-29 14:54:04.000000 elements-3.7.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-29 14:54:04.000000 elements-3.7.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.7.0/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.7.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-29 14:54:04.377231 elements-3.7.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.7.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-29 14:54:04.377231 elements-3.7.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.7.0/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.7.0/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.7.0/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1307 2024-05-22 06:01:09.000000 elements-3.7.0/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.7.0/tests/test_tree.py
```

### Comparing `elements-3.6.5/LICENSE` & `elements-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/PKG-INFO` & `elements-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.5
+Version: 3.7.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.5/README.md` & `elements-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/__init__.py` & `elements-3.7.0/elements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.6.5'
+__version__ = '3.7.0'
 
 from .agg import Agg
 from .checkpoint import Checkpoint, Saveable
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.6.5/elements/agg.py` & `elements-3.7.0/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/checkpoint.py` & `elements-3.7.0/elements/checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/config.py` & `elements-3.7.0/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/counter.py` & `elements-3.7.0/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/flags.py` & `elements-3.7.0/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/logger.py` & `elements-3.7.0/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/path.py` & `elements-3.7.0/elements/path.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,22 +103,26 @@
   def isdir(self):
     raise NotImplementedError
 
   def mkdirs(self):
     raise NotImplementedError
 
   def remove(self, recursive=False):
-    raise NotImplementedError
+    if recursive:
+      for path in reversed(list(self.glob('**'))):
+        path.remove()
+    else:
+      raise NotImplementedError
 
   def copy(self, dest, recursive=False):
-    raise NotImplementedError
+    _copy_across_filesystems(self, dest, recursive)
 
   def move(self, dest, recursive=False):
-    self.copy(dest)
-    self.remove()
+    self.copy(dest, recursive)
+    self.remove(recursive)
 
 
 class LocalPath(Path):
 
   __slots__ = ('_path',)
 
   def __init__(self, path):
@@ -148,24 +152,34 @@
   def mkdirs(self):
     os.makedirs(str(self), exist_ok=True)
 
   def remove(self, recursive=False):
     if recursive:
       shutil.rmtree(self)
     else:
-      os.rmdir(str(self)) if self.isdir() else os.remove(str(self))
+      if self.isdir():
+        os.rmdir(str(self))
+      else:
+        os.remove(str(self))
 
   def copy(self, dest, recursive=False):
-    if recursive:
-      shutil.copytree(self, type(self)(dest), dirs_exist_ok=True)
+    dest = Path(dest)
+    if isinstance(dest, type(self)):
+      shutil.copy2(self, type(self)(dest))
     else:
-      shutil.copy(self, type(self)(dest))
+      _copy_across_filesystems(self, dest, recursive)
 
   def move(self, dest, recursive=False):
-    shutil.move(self, dest)
+    dest = Path(dest)
+    print('TODO', type(self), type(dest))
+    if isinstance(dest, type(self)):
+      shutil.move(self, dest)
+    else:
+      _copy_across_filesystems(self, dest, recursive)
+      self.remove(recursive)
 
 
 class TFPath(Path):
 
   __slots__ = ('_path',)
 
   gfile = None
@@ -215,33 +229,26 @@
     if recursive:
       self.gfile.rmtree(str(self))
     else:
       self.gfile.remove(str(self))
 
   def copy(self, dest, recursive=False):
     dest = Path(dest)
-    if not recursive:
+    if isinstance(dest, type(self)) and not recursive:
       self.gfile.copy(str(self), str(dest), overwrite=True)
-      return
-    for folder, subdirs, files in self.gfile.walk(str(self)):
-      target = type(self)(folder.replace(str(self), str(dest)))
-      target.exists() or target.mkdirs()
-      for file in files:
-        (type(self)(folder) / file).copy(target / file)
+    else:
+      _copy_across_filesystems(self, dest, recursive)
 
   def move(self, dest, recursive=False):
     dest = Path(dest)
-    if recursive:
+    if isinstance(dest, type(self)) and not recursive:
       self.gfile.rename(self, str(dest), overwrite=True)
-      return
-    for folder, subdirs, files in self.gfile.walk(str(self)):
-      target = type(self)(folder.replace(str(self), str(dest)))
-      target.exists() or target.mkdirs()
-      for file in files:
-        (type(self)(folder) / file).move(target / file)
+    else:
+      _copy_across_filesystems(self, dest, recursive)
+      self.remove()
 
 
 class GCSPath(Path):
 
   __slots__ = ('_path', '_blob')
 
   client = None
@@ -382,54 +389,53 @@
   def remove(self, recursive=False):
     if recursive:
       for child in self.glob('**'):
         child.remove()
     else:
       self.blob.delete(self.client)
 
-  def move(self, dest, recursive=False):
+  def copy(self, dest, recursive=False):
     dest = Path(dest)
-    notgcs = not str(dest).startswith('gs://')
-    if recursive:
-      notgcs and dest.mkdirs()
-      for child in self.glob('**'):
-        name = str(child).removeprefix(str(self) + '/')
-        if child.isdir():
-          notgcs and dest.mkdirs()
-        else:
-          child.move(dest / name)
-    elif self._bucket(dest) == self.bucket.name:
-      dest = type(self)(dest)
-      self.bucket.rename_blob(self.blob, dest.blob.name)
+    if isinstance(dest, type(self)) and not recursive:
+      self.bucket.copy_blob(self.blob, dest.bucket, dest.blob.name)
     else:
-      self.copy(dest)
-      self.remove()
+      _copy_across_filesystems(self, dest, recursive)
 
-  def copy(self, dest, recursive=False):
+  def move(self, dest, recursive=False):
     dest = Path(dest)
-    notgcs = not str(dest).startswith('gs://')
-    if recursive:
-      notgcs and dest.mkdirs()
-      for child in self.glob('**'):
-        name = str(child).removeprefix(str(self) + '/')
-        if child.isdir():
-          notgcs and dest.mkdirs()
-        else:
-          child.copy(dest / name)
-    elif str(dest).startswith('gs://'):
-      dest = type(self)(dest)
-      self.bucket.copy_blob(self.blob, dest.bucket, dest.blob.name)
+    if isinstance(dest, type(self)) and not recursive:
+      if self.bucket.name == dest.bucket.name:
+        self.bucket.rename_blob(self.blob, dest.blob.name)
+      else:
+        self.bucket.copy_blob(self.blob, dest.bucket, dest.blob.name)
     else:
-      data = self.read('rb')
-      Path(dest).write(data, 'wb')
+      _copy_across_filesystems(self, dest, recursive)
+      self.remove()
 
   def _bucket(self, path):
     if not str(path).startswith('gs://'):
       return None
     return type(self)(path).bucket.name
 
 
+def _copy_across_filesystems(source, dest, recursive):
+  assert isinstance(source, Path), type(source)
+  assert isinstance(dest, Path), type(dest)
+  if not recursive:
+    assert source.isfile()
+    dest.write(source.read('rb'), 'wb')
+    return
+  prefix = str(source)
+  for s in source.glob('**'):
+    assert str(s).startswith(prefix), (source, s)
+    d = dest / str(s)[len(prefix):].lstrip('/')
+    if s.isdir():
+      d.mkdirs()
+    else:
+      d.write(s.read('rb'), 'wb')
+
+
 Path.filesystems = [
     (GCSPath, lambda path: path.startswith('gs://')),
     (TFPath, lambda path: path.startswith('/cns/')),
     (LocalPath, lambda path: True),
 ]
```

### Comparing `elements-3.6.5/elements/plotting.py` & `elements-3.7.0/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/printing.py` & `elements-3.7.0/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/rwlock.py` & `elements-3.7.0/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/timer.py` & `elements-3.7.0/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/tree.py` & `elements-3.7.0/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/usage.py` & `elements-3.7.0/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/uuid.py` & `elements-3.7.0/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements/when.py` & `elements-3.7.0/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/elements.egg-info/PKG-INFO` & `elements-3.7.0/elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.5
+Version: 3.7.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.5/elements.egg-info/SOURCES.txt` & `elements-3.7.0/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/setup.py` & `elements-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/tests/test_basics.py` & `elements-3.7.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/tests/test_checkpoint.py` & `elements-3.7.0/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/tests/test_flags.py` & `elements-3.7.0/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/tests/test_path.py` & `elements-3.7.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.5/tests/test_tree.py` & `elements-3.7.0/tests/test_tree.py`

 * *Files identical despite different names*

