# Comparing `tmp/pgn_clis-0.1.7.tar.gz` & `tmp/pgn_clis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_clis-0.1.7.tar", last modified: Wed May 29 16:04:35 2024, max compression
+gzip compressed data, was "pgn_clis-0.1.9.tar", last modified: Thu May 30 16:25:13 2024, max compression
```

## Comparing `pgn_clis-0.1.7.tar` & `pgn_clis-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.997525 pgn_clis-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 16:04:34.997525 pgn_clis-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-05-29 07:07:00.000000 pgn_clis-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      813 2024-05-29 16:04:32.000000 pgn_clis-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-29 16:04:34.997525 pgn_clis-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.987523 pgn_clis-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.987523 pgn_clis-0.1.7/src/pgn_clis/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-29 07:07:00.000000 pgn_clis-0.1.7/src/pgn_clis/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.987523 pgn_clis-0.1.7/src/pgn_clis/lib/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:42.000000 pgn_clis-0.1.7/src/pgn_clis/lib/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-29 07:13:23.000000 pgn_clis-0.1.7/src/pgn_clis/lib/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-29 09:00:48.000000 pgn_clis-0.1.7/src/pgn_clis/lib/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2266 2024-05-29 16:04:20.000000 pgn_clis-0.1.7/src/pgn_clis/lib/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-29 07:53:22.000000 pgn_clis-0.1.7/src/pgn_clis/lib/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-29 08:19:20.000000 pgn_clis-0.1.7/src/pgn_clis/lib/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.997525 pgn_clis-0.1.7/src/pgn_clis/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 07:13:52.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-29 07:14:41.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/clean.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-29 08:12:42.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/download.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1402 2024-05-29 16:01:16.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/random_samples.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-29 07:53:46.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/sans2ucis.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-29 08:19:54.000000 pgn_clis-0.1.7/src/pgn_clis/scripts/style_sans.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-29 16:04:34.997525 pgn_clis-0.1.7/src/pgn_clis.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      370 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-29 16:04:34.000000 pgn_clis-0.1.7/src/pgn_clis.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      427 2024-05-30 16:24:35.000000 pgn_clis-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      814 2024-05-30 16:25:09.000000 pgn_clis-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.195802 pgn_clis-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/src/pgn_clis/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/src/pgn_clis/lib/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      340 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2294 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/lib/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/src/pgn_clis/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      243 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/clean.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/download.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1402 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/random_samples.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      521 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/sans2ucis.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      526 2024-05-30 16:19:44.000000 pgn_clis-0.1.9/src/pgn_clis/scripts/style_sans.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 16:25:13.205803 pgn_clis-0.1.9/src/pgn_clis.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      765 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      651 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       36 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-30 16:25:13.000000 pgn_clis-0.1.9/src/pgn_clis.egg-info/top_level.txt
```

### Comparing `pgn_clis-0.1.7/pyproject.toml` & `pgn_clis-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pgn-clis"
-version = "0.1.7"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "package_description"
 dependencies = [
   "chess-utils", "chess-notation", "fs-tools"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/REPO.git"
+repo = "https://github.com/moveread/chess.git"
 
 [project.scripts]
 clean-pgns = "pgn_clis.scripts.clean:main"
 lichess-download = "pgn_clis.scripts.download:main"
 sans2ucis = "pgn_clis.scripts.sans2ucis:main"
 style-sans = "pgn_clis.scripts.style_sans:main"
 random-samples = "pgn_clis.scripts.random_samples:main"
```

### Comparing `pgn_clis-0.1.7/src/pgn_clis/lib/random_samples.py` & `pgn_clis-0.1.9/src/pgn_clis/lib/random_samples.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Sequence, NamedTuple, Iterable, TextIO
 import os
 import multiprocessing as mp
 import random
 import chess_utils as cu
+import chess_notation as cn
 import chess
 
 class Sample(NamedTuple):
   inputs: Sequence[str]
   ucis: Sequence[str]
 
 def random_sample(max_len: int = 150, rng = random.Random()) -> Sample:
```

### Comparing `pgn_clis-0.1.7/src/pgn_clis/scripts/random_samples.py` & `pgn_clis-0.1.9/src/pgn_clis/scripts/random_samples.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.7/src/pgn_clis/scripts/sans2ucis.py` & `pgn_clis-0.1.9/src/pgn_clis/scripts/sans2ucis.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.7/src/pgn_clis/scripts/style_sans.py` & `pgn_clis-0.1.9/src/pgn_clis/scripts/style_sans.py`

 * *Files identical despite different names*

### Comparing `pgn_clis-0.1.7/src/pgn_clis.egg-info/SOURCES.txt` & `pgn_clis-0.1.9/src/pgn_clis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

