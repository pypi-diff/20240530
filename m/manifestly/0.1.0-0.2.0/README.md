# Comparing `tmp/manifestly-0.1.0.tar.gz` & `tmp/manifestly-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifestly-0.1.0.tar", last modified: Thu May 30 16:54:51 2024, max compression
+gzip compressed data, was "manifestly-0.2.0.tar", last modified: Thu May 30 18:38:55 2024, max compression
```

## Comparing `manifestly-0.1.0.tar` & `manifestly-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.165125 manifestly-0.1.0/
--rw-r--r--   0 gdoermann   (501) staff       (20)     1070 2023-08-17 14:57:41.000000 manifestly-0.1.0/LICENSE
--rw-r--r--   0 gdoermann   (501) staff       (20)       15 2023-08-17 14:57:41.000000 manifestly-0.1.0/MANIFEST.in
--rw-r--r--   0 gdoermann   (501) staff       (20)    12028 2024-05-30 16:54:51.165032 manifestly-0.1.0/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)    10139 2024-05-30 16:14:43.000000 manifestly-0.1.0/README.md
--rw-r--r--   0 gdoermann   (501) staff       (20)      440 2024-05-30 16:53:18.000000 manifestly-0.1.0/pyproject.toml
--rw-r--r--   0 gdoermann   (501) staff       (20)     1824 2024-05-30 16:54:51.165397 manifestly-0.1.0/setup.cfg
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.161259 manifestly-0.1.0/src/
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.162846 manifestly-0.1.0/src/manifestly/
--rw-r--r--   0 gdoermann   (501) staff       (20)      305 2024-05-30 16:53:18.000000 manifestly-0.1.0/src/manifestly/__init__.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     5203 2024-05-29 21:52:04.000000 manifestly-0.1.0/src/manifestly/cli.py
--rw-r--r--   0 gdoermann   (501) staff       (20)    11874 2024-05-30 16:45:40.000000 manifestly-0.1.0/src/manifestly/core.py
--rw-r--r--   0 gdoermann   (501) staff       (20)      273 2024-05-29 19:42:44.000000 manifestly-0.1.0/src/manifestly/settings.py
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.164480 manifestly-0.1.0/src/manifestly.egg-info/
--rw-r--r--   0 gdoermann   (501) staff       (20)    12028 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/PKG-INFO
--rw-r--r--   0 gdoermann   (501) staff       (20)      429 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/SOURCES.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/dependency_links.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-29 18:41:38.000000 manifestly-0.1.0/src/manifestly.egg-info/not-zip-safe
--rw-r--r--   0 gdoermann   (501) staff       (20)      135 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/requires.txt
--rw-r--r--   0 gdoermann   (501) staff       (20)       17 2024-05-30 16:54:51.000000 manifestly-0.1.0/src/manifestly.egg-info/top_level.txt
-drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 16:54:51.164080 manifestly-0.1.0/src/tests/
--rw-r--r--   0 gdoermann   (501) staff       (20)        0 2024-05-30 14:09:14.000000 manifestly-0.1.0/src/tests/__init__.py
--rw-r--r--   0 gdoermann   (501) staff       (20)     8917 2024-05-30 16:51:42.000000 manifestly-0.1.0/src/tests/test_manifests.py
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 18:38:55.073862 manifestly-0.2.0/
+-rw-r--r--   0 gdoermann   (501) staff       (20)     1070 2023-08-17 14:57:41.000000 manifestly-0.2.0/LICENSE
+-rw-r--r--   0 gdoermann   (501) staff       (20)       15 2023-08-17 14:57:41.000000 manifestly-0.2.0/MANIFEST.in
+-rw-r--r--   0 gdoermann   (501) staff       (20)    12987 2024-05-30 18:38:55.073736 manifestly-0.2.0/PKG-INFO
+-rw-r--r--   0 gdoermann   (501) staff       (20)    10820 2024-05-30 18:36:11.000000 manifestly-0.2.0/README.md
+-rw-r--r--   0 gdoermann   (501) staff       (20)      440 2024-05-30 18:38:42.000000 manifestly-0.2.0/pyproject.toml
+-rw-r--r--   0 gdoermann   (501) staff       (20)     1891 2024-05-30 18:38:55.074136 manifestly-0.2.0/setup.cfg
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 18:38:55.069660 manifestly-0.2.0/src/
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 18:38:55.071314 manifestly-0.2.0/src/manifestly/
+-rw-r--r--   0 gdoermann   (501) staff       (20)      305 2024-05-30 18:38:42.000000 manifestly-0.2.0/src/manifestly/__init__.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)     5206 2024-05-30 18:20:53.000000 manifestly-0.2.0/src/manifestly/cli.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)    15342 2024-05-30 18:12:13.000000 manifestly-0.2.0/src/manifestly/core.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)      345 2024-05-30 17:09:17.000000 manifestly-0.2.0/src/manifestly/settings.py
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 18:38:55.073018 manifestly-0.2.0/src/manifestly.egg-info/
+-rw-r--r--   0 gdoermann   (501) staff       (20)    12987 2024-05-30 18:38:55.000000 manifestly-0.2.0/src/manifestly.egg-info/PKG-INFO
+-rw-r--r--   0 gdoermann   (501) staff       (20)      451 2024-05-30 18:38:55.000000 manifestly-0.2.0/src/manifestly.egg-info/SOURCES.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-30 18:38:55.000000 manifestly-0.2.0/src/manifestly.egg-info/dependency_links.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)        1 2024-05-29 18:41:38.000000 manifestly-0.2.0/src/manifestly.egg-info/not-zip-safe
+-rw-r--r--   0 gdoermann   (501) staff       (20)      198 2024-05-30 18:38:55.000000 manifestly-0.2.0/src/manifestly.egg-info/requires.txt
+-rw-r--r--   0 gdoermann   (501) staff       (20)       17 2024-05-30 18:38:55.000000 manifestly-0.2.0/src/manifestly.egg-info/top_level.txt
+drwxr-xr-x   0 gdoermann   (501) staff       (20)        0 2024-05-30 18:38:55.072684 manifestly-0.2.0/src/tests/
+-rw-r--r--   0 gdoermann   (501) staff       (20)        0 2024-05-30 14:09:14.000000 manifestly-0.2.0/src/tests/__init__.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)     6165 2024-05-30 18:24:54.000000 manifestly-0.2.0/src/tests/test_cli.py
+-rw-r--r--   0 gdoermann   (501) staff       (20)    12073 2024-05-30 18:10:27.000000 manifestly-0.2.0/src/tests/test_manifests.py
```

### Comparing `manifestly-0.1.0/LICENSE` & `manifestly-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manifestly-0.1.0/PKG-INFO` & `manifestly-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifestly
-Version: 0.1.0
+Version: 0.2.0
 Summary: Manifestly is a Python package designed to generate a manifest of a directory's contents, capturing file paths and their corresponding hashes. This allows for precise synchronization between two directories based on their content, ensuring that only files with differences in content are synchronized. This package provides a reliable solution for tracking and managing file changes efficiently.
 Home-page: https://github.com/gdoermann/manifestly
 Author: Greg Doermann
 Author-email: manifestly@doermann.me
 License: MIT
 Project-URL: Source, https://github.com/gdoermann/manifestly
 Project-URL: Tracker, https://github.com/gdoermann/manifestly/issues
@@ -18,19 +18,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: botocore~=1.29
-Requires-Dist: boto3~=1.26
 Requires-Dist: click
 Requires-Dist: fsspec
-Requires-Dist: s3fs
+Provides-Extra: aws
+Requires-Dist: s3fs; extra == "aws"
+Requires-Dist: boto3; extra == "aws"
+Requires-Dist: botocore; extra == "aws"
+Provides-Extra: gcs
+Requires-Dist: gcsfs; extra == "gcs"
+Requires-Dist: google-cloud-storage; extra == "gcs"
+Provides-Extra: azure
+Requires-Dist: adlfs; extra == "azure"
+Requires-Dist: azure-storage-blob; extra == "azure"
 Provides-Extra: extras
 Requires-Dist: tox~=4.14.2; extra == "extras"
 Requires-Dist: wheel; extra == "extras"
 Requires-Dist: ipython; extra == "extras"
 Requires-Dist: flake8~=6.0.0; extra == "extras"
 Requires-Dist: twine; extra == "extras"
 Requires-Dist: pytest; extra == "extras"
@@ -233,18 +240,33 @@
 ```bash
 s3://bucket/sync/prefix/.manifestly.json
 gcs://bucket/sync/prefix/.manifestly.json
 az://bucket/sync/prefix/.manifestly.json
 ```
 
 You may need to install the appropriate library for the remote path you are using.  
-For example, to use S3, you will need to install `s3fs`:
+For example, to use AWS, you will want to install the appropriate libraries.  
+I have provided some easy ways to do this with the extras:
 
 ```bash
-pip install s3fs
+pip install "manifestly[aws]"
+```
+
+This will install the `boto3` and `s3fs` libraries for you.
+
+To install google cloud storage:
+
+```bash
+pip install "manifestly[gcs]"
+```
+
+To install azure storage:
+
+```bash
+pip install "manifestly[azure]"
 ```
 
 # Module Usage
 
 Manifestly can also be run as a module from the command line. The following commands are available:
 
 ```bash
@@ -337,14 +359,21 @@
 * **SHA-3-384**: SHA3_384
 * **SHA-3-512**: SHA3_512
 * **SHAKE-128**: SHAKE_128
 * **SHAKE-256**: SHAKE_256
 * **BLAKE2b**: BLAKE2b
 * **BLAKE2s**: BLAKE2s
 
+# Ignore Files
+
+Manifestly supports the use of `.manifestignore` files to exclude specific files or directories from the manifest.
+The `.manifestignore` file should be placed in the root directory of the manifest and can contain patterns to match
+files or directories to exclude. This file is tracked by default and will be included in the manifest/synchronized
+when present.
+
 # Contributing
 
 We welcome contributions to Manifestly! If you would like to contribute, please fork the repository and submit a pull
 request.
 
 # License
```

### Comparing `manifestly-0.1.0/README.md` & `manifestly-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -193,18 +193,33 @@
 ```bash
 s3://bucket/sync/prefix/.manifestly.json
 gcs://bucket/sync/prefix/.manifestly.json
 az://bucket/sync/prefix/.manifestly.json
 ```
 
 You may need to install the appropriate library for the remote path you are using.  
-For example, to use S3, you will need to install `s3fs`:
+For example, to use AWS, you will want to install the appropriate libraries.  
+I have provided some easy ways to do this with the extras:
 
 ```bash
-pip install s3fs
+pip install "manifestly[aws]"
+```
+
+This will install the `boto3` and `s3fs` libraries for you.
+
+To install google cloud storage:
+
+```bash
+pip install "manifestly[gcs]"
+```
+
+To install azure storage:
+
+```bash
+pip install "manifestly[azure]"
 ```
 
 # Module Usage
 
 Manifestly can also be run as a module from the command line. The following commands are available:
 
 ```bash
@@ -297,14 +312,21 @@
 * **SHA-3-384**: SHA3_384
 * **SHA-3-512**: SHA3_512
 * **SHAKE-128**: SHAKE_128
 * **SHAKE-256**: SHAKE_256
 * **BLAKE2b**: BLAKE2b
 * **BLAKE2s**: BLAKE2s
 
+# Ignore Files
+
+Manifestly supports the use of `.manifestignore` files to exclude specific files or directories from the manifest.
+The `.manifestignore` file should be placed in the root directory of the manifest and can contain patterns to match
+files or directories to exclude. This file is tracked by default and will be included in the manifest/synchronized
+when present.
+
 # Contributing
 
 We welcome contributions to Manifestly! If you would like to contribute, please fork the repository and submit a pull
 request.
 
 # License
```

### Comparing `manifestly-0.1.0/setup.cfg` & `manifestly-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -28,26 +28,33 @@
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	botocore~=1.29
-	boto3~=1.26
 	click
 	fsspec
-	s3fs
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
+aws = 
+	s3fs
+	boto3
+	botocore
+gcs = 
+	gcsfs
+	google-cloud-storage
+azure = 
+	adlfs
+	azure-storage-blob
 extras = 
 	tox~=4.14.2
 	wheel
 	ipython
 	flake8~=6.0.0
 	twine
 	pytest
```

### Comparing `manifestly-0.1.0/src/manifestly/cli.py` & `manifestly-0.2.0/src/manifestly/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 Usage:
     manifestly generate <directory> [--hash-algorithm=<hash_algorithm>] [--output-file=<output_file>]
     manifestly sync <source_manifest> <target_manifest> <source_directory> <target_directory>
     manifestly compare <manifest1> <manifest2>
     manifestly patch <source_manifest> <target_manifest> <output_patch_file>
     manifestly pzip <source_manifest> <target_manifest> <output_zip_file>
 """
-import pathlib
-
 import click
 import fsspec
 
 from .core import Manifest
 
 
 @click.group()
@@ -40,15 +38,14 @@
         output_file = Manifest.default_manifest_file(directory)
     else:
         output_file = fsspec.open(output_file, 'w')
     Manifest.generate(directory, manifest_file=output_file, hash_algorithm=hash_algorithm)
     click.echo(f"Manifest saved to {output_file.path}")
 
 
-
 @cli.command('changed')
 @click.argument('manifest')
 @click.option('--root', default=None)
 def changed_cmd(manifest, root):
     """
     Print the files that have changed
     :param manifest: The manifest file
@@ -155,8 +152,8 @@
     """
     s_manifest = Manifest(source_manifest)
     s_manifest.pzip(target_manifest, output_zip_file)
     click.echo(f"Zip file saved to {output_zip_file}")
 
 
 if __name__ == '__main__':
-    cli()
+    cli()  # pragma: no cover
```

### Comparing `manifestly-0.1.0/src/manifestly/core.py` & `manifestly-0.2.0/src/manifestly/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,105 @@
 """
 Manifestly is a Python library for generating, loading, comparing, and syncing file manifests.
 
 This is the core module that provides the core functionality for generating, loading, comparing,
 and syncing file manifests.
 """
 
+import fnmatch
 import hashlib
-import io
 import json
 from itertools import chain
 from json import JSONDecodeError
 from typing import Union
 
 import fsspec
 from fsspec.core import OpenFile
 
 from manifestly import settings
 
 
+class ManifestlyIgnore:
+    """
+    Handles a .manifestlyignore file that works like a .gitignore file
+    You can specify files or directories to ignore.
+    This loads the .manifestlyignore file and provides a method to check if a file should be ignored.
+    """
+
+    def __init__(self, ignore_file: Union[str, OpenFile]):
+        if isinstance(ignore_file, str):
+            ignore_file = fsspec.open(ignore_file, 'r')
+        self.ignore_file = ignore_file
+        self.ignore_patterns = self.load_ignore_patterns()
+
+    def load_ignore_patterns(self):
+        """
+        Load the ignore patterns from the .manifestlyignore file
+        """
+        ignore = [settings.MANIFEST_NAME]
+        try:
+            with self.ignore_file.open() as f:
+                return ignore + [self.normalize_path(p) for p in f.read().splitlines()]
+        except FileNotFoundError:
+            return ignore
+
+    def should_ignore(self, file_path: str) -> bool:
+        """
+        Check if a file should be ignored.
+        :param file_path: The path to the file.
+        :return: True if the file should be ignored, False otherwise.
+        """
+        # Normalize the file path to always use forward slashes
+        normalized_path = self.normalize_path(file_path)
+
+        for pattern in self.ignore_patterns:
+            _pattern = pattern.strip('/')
+
+            if any(fnmatch.fnmatch(part, _pattern) for part in normalized_path.split('/')):
+                return True
+
+        return False
+
+    @staticmethod
+    def normalize_path(path: str) -> str:
+        """
+        Normalize a path to always use forward slashes
+        :param path: The path to normalize
+        :return: The normalized path
+        """
+        return path.replace('\\', '/')
+
+    def add_ignore_pattern(self, name: Union[str, OpenFile]):
+        """
+        Add an ignore pattern
+        :param name: pattern to ignore
+        """
+        if isinstance(name, OpenFile):
+            name = self.normalize_path(name.path).split('/')[-1]
+        if name not in self.ignore_patterns:
+            self.ignore_patterns.append(self.normalize_path(name))
+
+
 class Manifest:
     """
     A class to represent a manifest
     """
 
     def __init__(self, manifest_file: Union[str, OpenFile], manifest: dict = None,
-                 root: str = None):
+                 root: str = None, ignore: ManifestlyIgnore = None):
         if isinstance(manifest_file, str):
             manifest_file = fsspec.open(manifest_file)
         self.manifest_file: OpenFile = manifest_file
         self.manifest: dict = manifest
         self.root = root
         if self.manifest is None:
             self.load()
+        if ignore is None:
+            ignore = ManifestlyIgnore(self.default_ignore_file(self.root))
+        self.ignore = ignore
 
     def _reopen(self, mode='r'):
         return fsspec.open(self.manifest_file.path, mode)
 
     def save(self):
         """
         Save the manifest to a file
@@ -125,46 +189,73 @@
         :return: The path to the manifest file
         """
         fs, path = fsspec.core.url_to_fs(directory)
         manifest_path = fs.sep.join([path.rstrip(fs.sep), settings.MANIFEST_NAME])
         return fsspec.open(manifest_path)
 
     @classmethod
+    def default_ignore_file(cls, directory: Union[str, OpenFile]) -> OpenFile:
+        """
+        Get the default manifest file for a directory.
+        The directory must be a string or an fsspec.core.OpenFile object.
+
+        :param directory: The directory
+        :return: The path to the manifest file
+        """
+        fs, path = fsspec.core.url_to_fs(directory)
+        manifest_path = fs.sep.join([path.rstrip(fs.sep), settings.MANIFESTLY_IGNORE])
+        return fsspec.open(manifest_path, 'r')
+
+    @classmethod
     def generate(cls, directory, manifest_file: Union[str, OpenFile] = None, root_path: str = None,
-                 hash_algorithm=settings.DEFAULT_HASH_ALGORITHM) -> 'Manifest':
+                 hash_algorithm=settings.DEFAULT_HASH_ALGORITHM, ignore: ManifestlyIgnore = None) -> 'Manifest':
         """
         Generate a manifest for a directory
         :param directory: The directory to generate the manifest for
         :param manifest_file: Optional path to the manifest file
         :param root_path: The root path to use (all paths will be relative to this)
         :param hash_algorithm: Hash algorithm to use
+        :param ignore: The ignore file
         :return: The generated manifest
         """
         manifest = {}
         fs, path = fsspec.core.url_to_fs(directory)
         if root_path is None:
             root_path = path
         elif isinstance(root_path, OpenFile):
             root_path = root_path.path
 
+        # Load the ignore file if it exists
+        if ignore is None:
+            ignore = ManifestlyIgnore(cls.default_ignore_file(directory))
+        ignore.add_ignore_pattern(settings.MANIFEST_NAME)
+        if manifest_file:
+            if isinstance(manifest_file, OpenFile):
+                _ignore_file = manifest_file.path
+            else:
+                _ignore_file = manifest_file
+            _ignore_file = _ignore_file.split('/')[-1].split('\\')[-1]
+            ignore.add_ignore_pattern(_ignore_file)
+
         for file_path in fs.find(path):
             if fs.isfile(file_path):
-                if file_path.endswith(settings.MANIFEST_NAME):
+                # Check ignore patterns
+                if ignore.should_ignore(file_path):
                     continue
                 relative_path = file_path[len(root_path):].lstrip('/')
                 manifest[relative_path] = cls.calculate_hash(fs.open(file_path), algorithm=hash_algorithm)
 
         if manifest_file:
             if not isinstance(manifest_file, OpenFile):
                 manifest_file = fsspec.open(manifest_file, 'w')
             elif 'w' not in manifest_file.mode:
                 manifest_file = fsspec.open(manifest_file.path, 'w')
             with manifest_file as f:
                 json.dump(manifest, f, indent=2)
-        return cls(manifest_file, manifest, root=root_path)
+        return cls(manifest_file, manifest, root=root_path, ignore=ignore)
 
     def changed(self) -> dict:
         """
         Get the files that have changed
         This returns a dictionary of added, removed, and changed files
         :return: Dictionary of changed files
         """
@@ -180,15 +271,15 @@
             if not fs.exists(file_path):
                 changed['removed'][file] = _hash
                 continue
             _new_hash = self.calculate_hash(fs.open(file_path))
             if _hash != _new_hash:
                 changed['changed'][file] = _new_hash
         for file in fs.find(path):
-            if fs.isfile(file) and file.endswith(settings.MANIFEST_NAME):
+            if self.ignore.should_ignore(file):
                 continue
             relative_path = file[len(path):].lstrip('/')
             if relative_path not in self.manifest:
                 changed['added'][relative_path] = self.calculate_hash(fs.open(file))
         return changed
 
     def sync(self, target_manifest, dry_run=False) -> 'Manifest':
@@ -238,15 +329,16 @@
         """
         self.manifest = {}
         directory = self.root
         if directory is None:
             # Resolve the directory from the manifest file
             fs, path = fsspec.core.url_to_fs(self.manifest_file)  # noqa
             directory = fs._parent(path)  # noqa
-        _m = self.generate(directory=directory, manifest_file=self.manifest_file, root_path=self.root)
+        _m = self.generate(directory=directory, manifest_file=self.manifest_file, root_path=self.root,
+                           ignore=self.ignore)
         self.manifest = _m.manifest
 
     def diff(self, target_manifest) -> dict:
         """
         Compare the manifest with another manifest
         :param target_manifest: The path to the target manifest file or a Manifest object
         :return: A dictionary with the differences
```

### Comparing `manifestly-0.1.0/src/manifestly.egg-info/PKG-INFO` & `manifestly-0.2.0/src/manifestly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifestly
-Version: 0.1.0
+Version: 0.2.0
 Summary: Manifestly is a Python package designed to generate a manifest of a directory's contents, capturing file paths and their corresponding hashes. This allows for precise synchronization between two directories based on their content, ensuring that only files with differences in content are synchronized. This package provides a reliable solution for tracking and managing file changes efficiently.
 Home-page: https://github.com/gdoermann/manifestly
 Author: Greg Doermann
 Author-email: manifestly@doermann.me
 License: MIT
 Project-URL: Source, https://github.com/gdoermann/manifestly
 Project-URL: Tracker, https://github.com/gdoermann/manifestly/issues
@@ -18,19 +18,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: botocore~=1.29
-Requires-Dist: boto3~=1.26
 Requires-Dist: click
 Requires-Dist: fsspec
-Requires-Dist: s3fs
+Provides-Extra: aws
+Requires-Dist: s3fs; extra == "aws"
+Requires-Dist: boto3; extra == "aws"
+Requires-Dist: botocore; extra == "aws"
+Provides-Extra: gcs
+Requires-Dist: gcsfs; extra == "gcs"
+Requires-Dist: google-cloud-storage; extra == "gcs"
+Provides-Extra: azure
+Requires-Dist: adlfs; extra == "azure"
+Requires-Dist: azure-storage-blob; extra == "azure"
 Provides-Extra: extras
 Requires-Dist: tox~=4.14.2; extra == "extras"
 Requires-Dist: wheel; extra == "extras"
 Requires-Dist: ipython; extra == "extras"
 Requires-Dist: flake8~=6.0.0; extra == "extras"
 Requires-Dist: twine; extra == "extras"
 Requires-Dist: pytest; extra == "extras"
@@ -233,18 +240,33 @@
 ```bash
 s3://bucket/sync/prefix/.manifestly.json
 gcs://bucket/sync/prefix/.manifestly.json
 az://bucket/sync/prefix/.manifestly.json
 ```
 
 You may need to install the appropriate library for the remote path you are using.  
-For example, to use S3, you will need to install `s3fs`:
+For example, to use AWS, you will want to install the appropriate libraries.  
+I have provided some easy ways to do this with the extras:
 
 ```bash
-pip install s3fs
+pip install "manifestly[aws]"
+```
+
+This will install the `boto3` and `s3fs` libraries for you.
+
+To install google cloud storage:
+
+```bash
+pip install "manifestly[gcs]"
+```
+
+To install azure storage:
+
+```bash
+pip install "manifestly[azure]"
 ```
 
 # Module Usage
 
 Manifestly can also be run as a module from the command line. The following commands are available:
 
 ```bash
@@ -337,14 +359,21 @@
 * **SHA-3-384**: SHA3_384
 * **SHA-3-512**: SHA3_512
 * **SHAKE-128**: SHAKE_128
 * **SHAKE-256**: SHAKE_256
 * **BLAKE2b**: BLAKE2b
 * **BLAKE2s**: BLAKE2s
 
+# Ignore Files
+
+Manifestly supports the use of `.manifestignore` files to exclude specific files or directories from the manifest.
+The `.manifestignore` file should be placed in the root directory of the manifest and can contain patterns to match
+files or directories to exclude. This file is tracked by default and will be included in the manifest/synchronized
+when present.
+
 # Contributing
 
 We welcome contributions to Manifestly! If you would like to contribute, please fork the repository and submit a pull
 request.
 
 # License
```

