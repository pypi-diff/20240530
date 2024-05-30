# Comparing `tmp/pixe-0.7.2.tar.gz` & `tmp/pixe-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixe-0.7.2.tar", last modified: Mon Apr 29 01:51:13 2024, max compression
+gzip compressed data, was "pixe-0.7.3.tar", max compression
```

## Comparing `pixe-0.7.2.tar` & `pixe-0.7.3.tar`

### file list

```diff
@@ -1,24 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:13.146793 pixe-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 01:51:07.000000 pixe-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:51:13.146793 pixe-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 01:51:07.000000 pixe-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 01:51:07.000000 pixe-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:51:13.146793 pixe-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:13.142794 pixe-0.7.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:07.000000 pixe-0.7.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:13.142794 pixe-0.7.2/src/filetypes/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 01:51:07.000000 pixe-0.7.2/src/filetypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 01:51:07.000000 pixe-0.7.2/src/filetypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 01:51:07.000000 pixe-0.7.2/src/filetypes/image_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-29 01:51:07.000000 pixe-0.7.2/src/filetypes/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:13.142794 pixe-0.7.2/src/pixe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 01:51:13.000000 pixe-0.7.2/src/pixe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 01:51:07.000000 pixe-0.7.2/src/pixe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:51:13.142794 pixe-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-29 01:51:07.000000 pixe-0.7.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-29 01:51:07.000000 pixe-0.7.2/tests/test_unit.py
+-rw-r--r--   0        0        0    11357 2024-05-30 02:21:24.633336 pixe-0.7.3/LICENSE
+-rw-r--r--   0        0        0     3382 2024-05-30 02:21:24.634195 pixe-0.7.3/README.md
+-rw-r--r--   0        0        0     1018 2024-05-30 03:54:42.918130 pixe-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5302 2024-05-30 02:21:24.635166 pixe-0.7.3/src/pixe.py
+-rw-r--r--   0        0        0     4354 1970-01-01 00:00:00.000000 pixe-0.7.3/PKG-INFO
```

### Comparing `pixe-0.7.2/LICENSE` & `pixe-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixe-0.7.2/PKG-INFO` & `pixe-0.7.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.7.2
+Version: 0.7.3
 Summary: A digital helper to keep your files neat and tidy
-Author-email: Chris Wells <chris@ithuna.com>
-License: Apache License, Version 2.0
-Project-URL: homepage, https://github.com/ithuna/pixe.git
+License: Apache-2.0
 Keywords: archive,photos,organize
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
+Author: Chris Wells
+Author-email: ping@cwlls.dev
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Archiving
-Requires-Python: >=3.11
+Requires-Dist: Click (>=8.1.3,<9.0.0)
+Requires-Dist: Pillow (>=10.3.0,<11.0.0)
+Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
+Requires-Dist: piexif (>=1.1.3,<2.0.0)
+Requires-Dist: pillow-heif (>=0.16.0,<0.17.0)
+Requires-Dist: pyexiftool (>=0.5.0,<0.6.0)
+Project-URL: homepage, https://cwlls.dev/pixe
+Project-URL: repository, https://github.com/cwlls/pixe.git
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Click<8.2,>=8.1.3
-Requires-Dist: Pillow<10.4,>=10.3.0
-Requires-Dist: piexif<1.2,>=1.1.3
-Requires-Dist: ffmpeg-python<0.3.0,>=0.2.0
-Requires-Dist: pillow-heif>=0.16.0
-Requires-Dist: pyexiftool>=0.5.0
-Provides-Extra: tests
-Requires-Dist: pytest<7.3,>=7.2.1; extra == "tests"
-Requires-Dist: pytest-cov<4.1,>=4.0.0; extra == "tests"
-Requires-Dist: pytest-freezegun<0.5.0,>=0.4.2; extra == "tests"
-Requires-Dist: flake8<6.1,>=6.0.0; extra == "tests"
 
 # pixe
 [![flake8](https://github.com/ithuna/pixe/actions/workflows/flake8.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/flake8.yml) [![pytest](https://github.com/ithuna/pixe/actions/workflows/pytest.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/pytest.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A digital helper to keep your files neat and tidy.
 
 In its most basic invocation: `pixe <directory with files>` `pixe` will copy all JPG files from a source directory into a new set of subdirectories based on capture date. These files will also be renamed based on said capture date and a calculated SHA1 hash.
@@ -104,7 +102,8 @@
 overridden by specifying `--move`.
 
 #### --owner
 A string which will be inserted into the CameraOwnerName EXIF tag [0xa430]
 
 #### --copyright
 A string which will be inserted into the Copyright EXIF tag [0x8298]
+
```

### Comparing `pixe-0.7.2/README.md` & `pixe-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pixe-0.7.2/pyproject.toml` & `pixe-0.7.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-[project]
+[tool.poetry]
 name = "pixe"
-version = "0.7.2"
+version = "0.7.3"
 description = "A digital helper to keep your files neat and tidy"
 readme = "README.md"
-requires-python = ">=3.11"
-license = {text = "Apache License, Version 2.0"}
-keywords = ["archive", "photos", "organize"]
+license = "Apache-2.0"
+keywords = ["archive",
+	    "photos",
+	    "organize"
+]
 authors = [
-    {name = "Chris Wells", email = "chris@ithuna.com"},
+    "Chris Wells <ping@cwlls.dev>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
-    "Topic :: System :: Archiving",
-]
-dependencies = [
-    "Click>=8.1.3,<8.2",
-    "Pillow>=10.3.0,<10.4",
-    "piexif>=1.1.3,<1.2",
-    "ffmpeg-python>=0.2.0,<0.3.0",
-    "pillow-heif >=0.16.0",
-    "pyexiftool >=0.5.0",
+    "Topic :: System :: Archiving"
 ]
 
-[project.optional-dependencies]
-tests = [
-    "pytest>=7.2.1,<7.3",
-    "pytest-cov>=4.0.0,<4.1",
-    "pytest-freezegun>=0.4.2,<0.5.0",
-    "flake8>=6.0.0,<6.1",
-]
+[tool.poetry.dependencies]
+Python = "^3.11"
+Click = "^8.1.3"
+Pillow = "^10.3.0"
+piexif = "^1.1.3"
+ffmpeg-python = "^0.2.0"
+pillow-heif = "^0.16.0"
+pyexiftool = "^0.5.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.1"
+pytest-cov = "^4.0.0"
+pytest-freezegun = "^0.4.2"
+flake8 = "^6.0.0"
 
-[project.urls]
-homepage = "https://github.com/ithuna/pixe.git"
+[tool.poetry.urls]
+homepage = "https://cwlls.dev/pixe"
+repository = "https://github.com/cwlls/pixe.git"
 
-[project.scripts]
+[tool.poetry.scripts]
 pixe = "pixe:cli"
 
-[tool.setuptools.dynamic]
-version = {attr = "package.__version__"}
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonary.api"
```

### Comparing `pixe-0.7.2/src/pixe.py` & `pixe-0.7.3/src/pixe.py`

 * *Files identical despite different names*

