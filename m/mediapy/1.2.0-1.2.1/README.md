# Comparing `tmp/mediapy-1.2.0.tar.gz` & `tmp/mediapy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediapy-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mediapy-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediapy-1.2.0.tar` & `mediapy-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11358 2023-12-06 10:06:23.913385 mediapy-1.2.0/LICENSE
--rw-r--r--   0        0        0     3738 2023-12-06 10:06:23.913385 mediapy-1.2.0/README.md
--rw-r--r--   0        0        0    68424 2023-12-06 10:06:23.913385 mediapy-1.2.0/mediapy/__init__.py
--rw-r--r--   0        0        0        0 2023-12-06 10:06:23.913385 mediapy-1.2.0/mediapy/py.typed
--rw-r--r--   0        0        0     2389 2023-12-06 10:06:23.917385 mediapy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 mediapy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-30 12:53:40.740832 mediapy-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3738 2024-05-30 12:53:40.740832 mediapy-1.2.1/README.md
+-rw-r--r--   0        0        0    68644 2024-05-30 12:53:40.740832 mediapy-1.2.1/mediapy/__init__.py
+-rw-r--r--   0        0        0     9697 2024-05-30 12:53:40.740832 mediapy-1.2.1/mediapy/mediapy_examples.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:53:40.740832 mediapy-1.2.1/mediapy/py.typed
+-rw-r--r--   0        0        0     2600 2024-05-30 12:53:40.744832 mediapy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 mediapy-1.2.1/PKG-INFO
```

### Comparing `mediapy-1.2.0/LICENSE` & `mediapy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mediapy-1.2.0/README.md` & `mediapy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mediapy-1.2.0/mediapy/__init__.py` & `mediapy-1.2.1/mediapy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 The mediapy Authors.
+# Copyright 2024 The mediapy Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -100,26 +100,27 @@
       w.add_image(darken_image(image))
 ```
 """
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import base64
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import functools
 import importlib
 import io
 import itertools
 import math
 import numbers
+import os  # Package only needed for typing.TYPE_CHECKING.
 import pathlib
 import re
 import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
@@ -130,19 +131,17 @@
 import IPython.display
 import matplotlib.pyplot
 import numpy as np
 import numpy.typing as npt
 import PIL.Image
 import PIL.ImageOps
 
-if typing.TYPE_CHECKING:
-  import os  # pylint: disable=g-bad-import-order
 
 if not hasattr(PIL.Image, 'Resampling'):  # Allow Pillow<9.0.
-  PIL.Image.Resampling = PIL.Image
+  PIL.Image.Resampling = PIL.Image  # type: ignore
 
 # Selected and reordered here for pdoc documentation.
 __all__ = [
     'show_image',
     'show_images',
     'compare_images',
     'show_video',
@@ -185,15 +184,15 @@
   _ArrayLike = typing.TypeVar('_ArrayLike')
   _DTypeLike = typing.TypeVar('_DTypeLike')
   _NDArray = typing.TypeVar('_NDArray')
   _DType = typing.TypeVar('_DType')  # pylint: disable=invalid-name
 
 _IPYTHON_HTML_SIZE_LIMIT = 20_000_000
 _T = typing.TypeVar('_T')
-_Path = typing.Union[str, 'os.PathLike[str]']
+_Path = typing.Union[str, os.PathLike[str]]
 
 _IMAGE_COMPARISON_HTML = """\
 <script
   defer
   src="https://unpkg.com/img-comparison-slider@7/dist/index.js"
 ></script>
 <link
@@ -416,15 +415,16 @@
     elif dst_max <= np.iinfo(np.uint32).max:
       result = (a.astype(np.float64) * (dst_max / src_max) + 0.5).astype(dtype)
     else:
       # https://stackoverflow.com/a/66306123/
       a = a.astype(np.float64) * (dst_max / src_max) + 0.5
       dst = np.atleast_1d(a)
       values_too_large = dst >= np.float64(dst_max)
-      dst = dst.astype(dtype)
+      with np.errstate(invalid='ignore'):
+        dst = dst.astype(dtype)
       dst[values_too_large] = dst_max
       result = dst if a.ndim > 0 else dst[0]
   else:
     assert np.issubdtype(dtype, np.floating)
     result = a.astype(dtype)
     if np.issubdtype(a.dtype, np.unsignedinteger):
       result = result / dtype.type(np.iinfo(a.dtype).max)
@@ -602,15 +602,16 @@
 
 
 def _pil_image(image: _ArrayLike, mode: str | None = None) -> PIL.Image.Image:
   """Returns a PIL image given a numpy matrix (either uint8 or float [0,1])."""
   image = _as_valid_media_array(image)
   if image.ndim not in (2, 3):
     raise ValueError(f'Image shape {image.shape} is neither 2D nor 3D.')
-  return PIL.Image.fromarray(image, mode=mode)
+  pil_image: PIL.Image.Image = PIL.Image.fromarray(image, mode=mode)  # type: ignore[no-untyped-call]
+  return pil_image
 
 
 def resize_image(image: _ArrayLike, shape: tuple[int, int]) -> _NDArray:
   """Resizes image to specified spatial dimensions using a Lanczos filter.
 
   Args:
     image: Array-like 2D or 3D object, where dtype is uint or floating-point.
@@ -880,17 +881,19 @@
     data: Buffer containing compressed image.
     dtype: Data type of the returned array.  If None, `np.uint8` or `np.uint16`
       is inferred automatically.
     apply_exif_transpose: If True, rotate image according to EXIF orientation.
   """
   pil_image = PIL.Image.open(io.BytesIO(data))
   if apply_exif_transpose:
-    pil_image = PIL.ImageOps.exif_transpose(pil_image)
+    tmp_image = PIL.ImageOps.exif_transpose(pil_image)  # Future: in_place=True.
+    assert tmp_image
+    pil_image = tmp_image
   if dtype is None:
-    dtype = np.uint16 if pil_image.mode == 'I' else np.uint8
+    dtype = np.uint16 if pil_image.mode.startswith('I') else np.uint8
   return np.array(pil_image, dtype=dtype)
 
 
 def html_from_compressed_image(
     data: bytes,
     width: int,
     height: int,
@@ -1181,15 +1184,16 @@
 
 class VideoMetadata(typing.NamedTuple):
   """Represents the data stored in a video container header.
 
   Attributes:
     num_images: Number of frames that is expected from the video stream.  This
       is estimated from the framerate and the duration stored in the video
-      header, so it might be inexact.
+      header, so it might be inexact.  We set the value to -1 if number of
+      frames is not found in the header.
     shape: The dimensions (height, width) of each video frame.
     fps: The framerate in frames per second.
     bps: The estimated bitrate of the video stream in bits per second, retrieved
       from the video header.
   """
 
   num_images: int
@@ -1217,35 +1221,35 @@
   ]
   with subprocess.Popen(
       command, stderr=subprocess.PIPE, encoding='utf-8'
   ) as proc:
     _, err = proc.communicate()
   bps = fps = num_images = width = height = rotation = None
   for line in err.split('\n'):
-    if match := re.search(r', bitrate: *([0-9.]+) kb/s', line):
+    if match := re.search(r', bitrate: *([\d.]+) kb/s', line):
       bps = int(match.group(1)) * 1000
-    if matches := re.findall(r'frame= *([0-9]+) ', line):
+    if matches := re.findall(r'frame= *(\d+) ', line):
       num_images = int(matches[-1])
     if 'Stream #0:' in line and ': Video:' in line:
-      if not (match := re.search(r', ([0-9]+)x([0-9]+)', line)):
+      if not (match := re.search(r', (\d+)x(\d+)', line)):
         raise RuntimeError(f'Unable to parse video dimensions in line {line}')
       width, height = int(match.group(1)), int(match.group(2))
-      if match := re.search(r', ([0-9.]+) fps', line):
+      if match := re.search(r', ([\d.]+) fps', line):
         fps = float(match.group(1))
       elif str(path).endswith('.gif'):
         # Some GIF files lack a framerate attribute; use a reasonable default.
         fps = 10
       else:
         raise RuntimeError(f'Unable to parse video framerate in line {line}')
     if match := re.fullmatch(r'\s*rotate\s*:\s*(\d+)', line):
       rotation = int(match.group(1))
     if match := re.fullmatch(r'.*rotation of (-?\d+).*\sdegrees', line):
       rotation = int(match.group(1))
   if not num_images:
-    raise RuntimeError(f'Unable to find frames in video: {err}')
+    num_images = -1
   if not width:
     raise RuntimeError(f'Unable to parse video header: {err}')
   # By default, ffmpeg enables "-autorotate"; we just fix the dimensions.
   if rotation in (90, 270, -90, -270):
     width, height = height, width
   assert height is not None and width is not None
   shape = height, width
```

### Comparing `mediapy-1.2.0/pyproject.toml` & `mediapy-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,19 @@
 strict = true
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "mediapy_test"
 ignore_errors = true
 
+[[tool.mypy.overrides]]
+module = "mediapy_examples"
+disallow_untyped_calls = false
+disallow_untyped_defs = false
+
 [tool.pyink]
 # Formatting configuration to follow Google style-guide.
 line-length = 80
 preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
 # Ignore both *.ipynb and .ipynb_checkpoints/.
@@ -74,18 +79,20 @@
 
 [tool.pylint.main]
 disable = [
     "unspecified-encoding", "line-too-long", "too-many-lines",
     "too-few-public-methods", "too-many-locals", "too-many-instance-attributes",
     "too-many-branches", "too-many-statements", "too-many-arguments",
     "using-constant-test", "wrong-import-order", "use-dict-literal",
+    "missing-module-docstring",
 ]
 reports = false
 score = false
 recursive = true
+ignore-paths = [".*ipynb_checkpoints", "^.pytype", ".*/.pytype"]
 
 [tool.pylint.basic]
 good-names-rgxs = "^[a-z][a-z0-9]?|[A-Z]([A-Z_]*[A-Z])?$"
 
 [tool.pylint.format]
 indent-string = "  "
 expected-line-ending-format = "LF"
```

### Comparing `mediapy-1.2.0/PKG-INFO` & `mediapy-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediapy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Read/write/show images and videos in an IPython notebook
 Keywords: 
 Author-email: Google LLC <mediapy-owners@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

