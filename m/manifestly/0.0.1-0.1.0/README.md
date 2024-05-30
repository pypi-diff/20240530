# Comparing `tmp/manifestly-0.0.1.tar.gz` & `tmp/manifestly-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifestly-0.0.1.tar", last modified: Wed May 29 22:09:36 2024, max compression
+gzip compressed data, was "manifestly-0.1.0.tar", last modified: Thu May 30 16:54:51 2024, max compression
```

## Comparing `manifestly-0.0.1.tar` & `manifestly-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-29 22:09:36.589692 manifestly-0.0.1/
--rw-r--r--   0 gdoermann   (501) staff       (20)     1070 2023-08-17 14:57:41.000000 manifestly-0.0.1/LICENSE
--rw-r--r--   0 gdoermann   (501) staff       (20)       15 2023-08-17 14:57:41.000000 manifestly-0.0.1/MANIFEST.in
--rw-r--r--   0 gdoermann   (501) staff       (20)    12026 2024-05-29 22:09:36.589611 manifestly-0.0.1/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)    10137 2024-05-29 21:53:32.000000 manifestly-0.0.1/README.md
--rw-r--r--   0 gdoermann   (501) staff       (20)      440 2024-05-29 17:09:55.000000 manifestly-0.0.1/pyproject.toml
--rw-r--r--   0 gdoermann   (501) staff       (20)     1801 2024-05-29 22:09:36.589962 manifestly-0.0.1/setup.cfg
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-29 22:09:36.586372 manifestly-0.0.1/src/
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-29 22:09:36.587884 manifestly-0.0.1/src/manifestly/
--rw-r--r--   0 gdoermann   (501) staff       (20)      305 2024-05-29 19:48:25.000000 manifestly-0.0.1/src/manifestly/__init__.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     5203 2024-05-29 21:52:04.000000 manifestly-0.0.1/src/manifestly/cli.py
--rw-r--r--   0 gdoermann   (501) staff       (20)    10749 2024-05-29 22:05:46.000000 manifestly-0.0.1/src/manifestly/core.py
--rw-r--r--   0 gdoermann   (501) staff       (20)      273 2024-05-29 19:42:44.000000 manifestly-0.0.1/src/manifestly/settings.py
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-29 22:09:36.589089 manifestly-0.0.1/src/manifestly.egg-info/
--rw-r--r--   0 gdoermann   (501) staff       (20)    12026 2024-05-29 22:09:36.000000 manifestly-0.0.1/src/manifestly.egg-info/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)      379 2024-05-29 22:09:36.000000 manifestly-0.0.1/src/manifestly.egg-info/SOURCES.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-29 22:09:36.000000 manifestly-0.0.1/src/manifestly.egg-info/dependency_links.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-29 18:41:38.000000 manifestly-0.0.1/src/manifestly.egg-info/not-zip-safe
--rw-r--r--   0 gdoermann   (501) staff       (20)      135 2024-05-29 22:09:36.000000 manifestly-0.0.1/src/manifestly.egg-info/requires.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)       11 2024-05-29 22:09:36.000000 manifestly-0.0.1/src/manifestly.egg-info/top_level.txt
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.165125 manifestly-0.1.0/
+-rw-r--r--   0 gdoermann   (501) staff       (20)     1070 2023-08-17 14:57:41.000000 manifestly-0.1.0/LICENSE
+-rw-r--r--   0 gdoermann   (501) staff       (20)       15 2023-08-17 14:57:41.000000 manifestly-0.1.0/MANIFEST.in
+-rw-r--r--   0 gdoermann   (501) staff       (20)    12028 2024-05-30 16:54:51.165032 manifestly-0.1.0/PKG-INFO
+-rw-r--r--   0 gdoermann   (501) staff       (20)    10139 2024-05-30 16:14:43.000000 manifestly-0.1.0/README.md
+-rw-r--r--   0 gdoermann   (501) staff       (20)      440 2024-05-30 16:53:18.000000 manifestly-0.1.0/pyproject.toml
+-rw-r--r--   0 gdoermann   (501) staff       (20)     1824 2024-05-30 16:54:51.165397 manifestly-0.1.0/setup.cfg
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.161259 manifestly-0.1.0/src/
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.162846 manifestly-0.1.0/src/manifestly/
+-rw-r--r--   0 gdoermann   (501) staff       (20)      305 2024-05-30 16:53:18.000000 manifestly-0.1.0/src/manifestly/__init__.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)     5203 2024-05-29 21:52:04.000000 manifestly-0.1.0/src/manifestly/cli.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)    11874 2024-05-30 16:45:40.000000 manifestly-0.1.0/src/manifestly/core.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)      273 2024-05-29 19:42:44.000000 manifestly-0.1.0/src/manifestly/settings.py
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.164480 manifestly-0.1.0/src/manifestly.egg-info/
+-rw-r--r--   0 gdoermann   (501) staff       (20)    12028 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/PKG-INFO
+-rw-r--r--   0 gdoermann   (501) staff       (20)      429 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/SOURCES.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/dependency_links.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-29 18:41:38.000000 manifestly-0.1.0/src/manifestly.egg-info/not-zip-safe
+-rw-r--r--   0 gdoermann   (501) staff       (20)      135 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/requires.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)       17 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/top_level.txt
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.164080 manifestly-0.1.0/src/tests/
+-rw-r--r--   0 gdoermann   (501) staff       (20)        0 2024-05-30 14:09:14.000000 manifestly-0.1.0/src/tests/__init__.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)     8917 2024-05-30 16:51:42.000000 manifestly-0.1.0/src/tests/test_manifests.py
```

### Comparing `manifestly-0.0.1/LICENSE` & `manifestly-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manifestly-0.0.1/PKG-INFO` & `manifestly-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifestly
-Version: 0.0.1
+Version: 0.1.0
 Summary: Manifestly is a Python package designed to generate a manifest of a directory's contents, capturing file paths and their corresponding hashes. This allows for precise synchronization between two directories based on their content, ensuring that only files with differences in content are synchronized. This package provides a reliable solution for tracking and managing file changes efficiently.
 Home-page: https://github.com/gdoermann/manifestly
 Author: Greg Doermann
 Author-email: manifestly@doermann.me
 License: MIT
 Project-URL: Source, https://github.com/gdoermann/manifestly
 Project-URL: Tracker, https://github.com/gdoermann/manifestly/issues
@@ -68,16 +68,16 @@
 To generate a manifest for a directory:
 
 ```python
 import manifestly
 
 directory_to_scan = "path/to/your/directory"
 output_file = ".manifestly.json"
-manifest = manifestly.Manifest.generate(directory_to_scan)
-manifest.save(output_file)
+manifest = manifestly.Manifest.generate(directory_to_scan, output_file)
+manifest.save()
 print(f"Manifest saved to {output_file}")
 ```
 
 Or through the cli:
 
 ```bash
 python -m manifestly.cli generate [--output-file .manifestly.json] path/to/your/directory
```

### Comparing `manifestly-0.0.1/README.md` & `manifestly-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 To generate a manifest for a directory:
 
 ```python
 import manifestly
 
 directory_to_scan = "path/to/your/directory"
 output_file = ".manifestly.json"
-manifest = manifestly.Manifest.generate(directory_to_scan)
-manifest.save(output_file)
+manifest = manifestly.Manifest.generate(directory_to_scan, output_file)
+manifest.save()
 print(f"Manifest saved to {output_file}")
 ```
 
 Or through the cli:
 
 ```bash
 python -m manifestly.cli generate [--output-file .manifestly.json] path/to/your/directory
```

### Comparing `manifestly-0.0.1/setup.cfg` & `manifestly-0.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gdoermann/manifestly
 author = Greg Doermann
 author_email = manifestly@doermann.me
 license = MIT
 license_file = LICENSE
+test_suite = src/tests
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `manifestly-0.0.1/src/manifestly/cli.py` & `manifestly-0.1.0/src/manifestly/cli.py`

 * *Files identical despite different names*

### Comparing `manifestly-0.0.1/src/manifestly/core.py` & `manifestly-0.1.0/src/manifestly/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,79 +2,118 @@
 Manifestly is a Python library for generating, loading, comparing, and syncing file manifests.
 
 This is the core module that provides the core functionality for generating, loading, comparing,
 and syncing file manifests.
 """
 
 import hashlib
+import io
 import json
 from itertools import chain
+from json import JSONDecodeError
 from typing import Union
 
 import fsspec
 from fsspec.core import OpenFile
 
 from manifestly import settings
 
 
 class Manifest:
     """
     A class to represent a manifest
     """
 
-    def __init__(self, manifest_file: Union[str, OpenFile], manifest=None,
+    def __init__(self, manifest_file: Union[str, OpenFile], manifest: dict = None,
                  root: str = None):
         if isinstance(manifest_file, str):
             manifest_file = fsspec.open(manifest_file)
         self.manifest_file: OpenFile = manifest_file
-        self.manifest = manifest
+        self.manifest: dict = manifest
         self.root = root
         if self.manifest is None:
             self.load()
 
-    def save(self, file_path):
+    def _reopen(self, mode='r'):
+        return fsspec.open(self.manifest_file.path, mode)
+
+    def save(self):
         """
         Save the manifest to a file
-        :param file_path: The path to the file
+        :param file_path: The path to the manifest file
         """
-        if not isinstance(file_path, OpenFile):
-            file_path = fsspec.open(file_path, 'w')
-        # Check if we are in write mode...
-        if 'w' not in file_path.mode:
-            # Reopen in write mode
-            file_path = fsspec.open(file_path.path, 'w')
+        _file = self._reopen('w')
         # Make sure directories exist
-        file_path.fs.makedirs(file_path.fs._parent(file_path.path), exist_ok=True)
+        _file.fs.makedirs(_file.fs._parent(_file.path), exist_ok=True)
 
-        with file_path.open() as f:
+        with _file.open() as f:
+            f.seek(0)
             json.dump(self.manifest, f, indent=2)
 
     def items(self):
         """
         Get the items in the manifest
         :return:
         """
         return self.manifest.items()
 
+    def keys(self):
+        """
+        Get the keys in the manifest
+        :return:
+        """
+        return self.manifest.keys()
+
+    def values(self):
+        """
+        Get the values in the manifest
+        :return:
+        """
+        return self.manifest.values()
+
+    def __eq__(self, other):
+        """
+        Check if the manifest is equal to another manifest
+        :param other: The other manifest
+        :return: True if the manifests are equal, False otherwise
+        """
+        if not isinstance(other, Manifest):
+            return False
+        return self.manifest == other.manifest
+
+    def __contains__(self, item):
+        """
+        Check if the manifest contains a file
+        :param item: The file to check
+        :return: True if the file is in the manifest, False otherwise
+        """
+        return item in self.manifest
+
     def load(self):
         """
         Load a manifest from a file
         :return: The loaded manifest
         """
         try:
-            with self.manifest_file as f:
-                self.manifest = json.load(f)
+            with self._reopen() as f:
+                _data = f.read()
+                if not _data:
+                    self.manifest = {}
+                else:
+                    self.manifest = json.loads(_data)
         except FileNotFoundError:
             self.manifest = {}
-            self.save(self.manifest_file)
+            self.save()
         except IsADirectoryError:
             # The manifest file is a directory, so we need to append the default manifest file name
             self.root = self.manifest_file
             self.manifest_file = self.default_manifest_file(self.manifest_file)
             self.load()
+        except JSONDecodeError:
+            self.manifest = {}
         if self.root is None:
             # Resolve the root path from the manifest file
             fs, path = fsspec.core.url_to_fs(self.manifest_file)
             self.root = fs._parent(path)
 
     @classmethod
     def default_manifest_file(cls, directory: Union[str, OpenFile]) -> OpenFile:
@@ -100,14 +139,16 @@
         :param hash_algorithm: Hash algorithm to use
         :return: The generated manifest
         """
         manifest = {}
         fs, path = fsspec.core.url_to_fs(directory)
         if root_path is None:
             root_path = path
+        elif isinstance(root_path, OpenFile):
+            root_path = root_path.path
 
         for file_path in fs.find(path):
             if fs.isfile(file_path):
                 if file_path.endswith(settings.MANIFEST_NAME):
                     continue
                 relative_path = file_path[len(root_path):].lstrip('/')
                 manifest[relative_path] = cls.calculate_hash(fs.open(file_path), algorithm=hash_algorithm)
@@ -146,15 +187,15 @@
             if fs.isfile(file) and file.endswith(settings.MANIFEST_NAME):
                 continue
             relative_path = file[len(path):].lstrip('/')
             if relative_path not in self.manifest:
                 changed['added'][relative_path] = self.calculate_hash(fs.open(file))
         return changed
 
-    def sync(self, target_manifest, dry_run=False):
+    def sync(self, target_manifest, dry_run=False) -> 'Manifest':
         """
         Sync the target directory to match the source manifest
         :param target_manifest: The path to the target manifest file or a Manifest object
         :param dry_run: Perform a dry run
         """
         if isinstance(target_manifest, str):
             target_manifest = Manifest(target_manifest)
@@ -185,26 +226,28 @@
                     print(f'Remove {target_file}')
                     continue
                 fs_target.rm(target_file)
 
         if not dry_run:
             # Regenerate the target manifest
             target_manifest.refresh()
+        return target_manifest
 
     def refresh(self):
         """
         Regenerate the manifest
         """
         self.manifest = {}
         directory = self.root
         if directory is None:
             # Resolve the directory from the manifest file
             fs, path = fsspec.core.url_to_fs(self.manifest_file)  # noqa
             directory = fs._parent(path)  # noqa
-        self.generate(directory=directory, manifest_file=self.manifest_file, root_path=self.root)
+        _m = self.generate(directory=directory, manifest_file=self.manifest_file, root_path=self.root)
+        self.manifest = _m.manifest
 
     def diff(self, target_manifest) -> dict:
         """
         Compare the manifest with another manifest
         :param target_manifest: The path to the target manifest file or a Manifest object
         :return: A dictionary with the differences
         """
@@ -212,20 +255,20 @@
             target_manifest = Manifest(target_manifest)
         diff = {
             'added': {},
             'removed': {},
             'changed': {}
         }
         for file, _hash in self.items():
-            if file not in target_manifest.items():
+            if file not in target_manifest.manifest:
                 diff['added'][file] = _hash
-            elif target_manifest.items()[file] != _hash:
+            elif target_manifest.manifest[file] != _hash:
                 diff['changed'][file] = _hash
         for file, _hash in target_manifest.items():
-            if file not in self.items():
+            if file not in self.manifest:
                 diff['removed'][file] = _hash
         return diff
 
     def patch(self, target_manifest, output_patch_file) -> dict:
         """
         Generate a patch file that can be used to update the target manifest to match the source manifest.
         :param target_manifest: The path to the target manifest file or a Manifest object
```

### Comparing `manifestly-0.0.1/src/manifestly.egg-info/PKG-INFO` & `manifestly-0.1.0/src/manifestly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifestly
-Version: 0.0.1
+Version: 0.1.0
 Summary: Manifestly is a Python package designed to generate a manifest of a directory's contents, capturing file paths and their corresponding hashes. This allows for precise synchronization between two directories based on their content, ensuring that only files with differences in content are synchronized. This package provides a reliable solution for tracking and managing file changes efficiently.
 Home-page: https://github.com/gdoermann/manifestly
 Author: Greg Doermann
 Author-email: manifestly@doermann.me
 License: MIT
 Project-URL: Source, https://github.com/gdoermann/manifestly
 Project-URL: Tracker, https://github.com/gdoermann/manifestly/issues
@@ -68,16 +68,16 @@
 To generate a manifest for a directory:
 
 ```python
 import manifestly
 
 directory_to_scan = "path/to/your/directory"
 output_file = ".manifestly.json"
-manifest = manifestly.Manifest.generate(directory_to_scan)
-manifest.save(output_file)
+manifest = manifestly.Manifest.generate(directory_to_scan, output_file)
+manifest.save()
 print(f"Manifest saved to {output_file}")
 ```
 
 Or through the cli:
 
 ```bash
 python -m manifestly.cli generate [--output-file .manifestly.json] path/to/your/directory
```

