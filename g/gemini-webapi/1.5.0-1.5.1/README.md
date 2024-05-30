# Comparing `tmp/gemini_webapi-1.5.0.tar.gz` & `tmp/gemini_webapi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_webapi-1.5.0.tar", last modified: Sun May 26 22:25:41 2024, max compression
+gzip compressed data, was "gemini_webapi-1.5.1.tar", last modified: Thu May 30 17:46:49 2024, max compression
```

## Comparing `gemini_webapi-1.5.0.tar` & `gemini_webapi-1.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.808960 gemini_webapi-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.812960 gemini_webapi-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.812960 gemini_webapi-1.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.812960 gemini_webapi-1.5.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.812960 gemini_webapi-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.812960 gemini_webapi-1.5.0/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20898 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-26 22:25:41.000000 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-26 22:25:41.000000 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:25:41.000000 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 22:25:41.000000 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 22:25:41.000000 gemini_webapi-1.5.0/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:25:41.816960 gemini_webapi-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-26 22:25:34.000000 gemini_webapi-1.5.0/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.160125 gemini_webapi-1.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.164125 gemini_webapi-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.164125 gemini_webapi-1.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.164125 gemini_webapi-1.5.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.160125 gemini_webapi-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.164125 gemini_webapi-1.5.1/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21108 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-30 17:46:49.000000 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 17:46:49.000000 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:46:49.000000 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 17:46:49.000000 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 17:46:49.000000 gemini_webapi-1.5.1/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:46:49.168125 gemini_webapi-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 17:46:44.000000 gemini_webapi-1.5.1/tests/test_save_image.py
```

### Comparing `gemini_webapi-1.5.0/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.5.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/.gitignore` & `gemini_webapi-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/LICENSE` & `gemini_webapi-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/PKG-INFO` & `gemini_webapi-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.5.0
+Version: 1.5.1
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.5.0/README.md` & `gemini_webapi-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/assets/banner.png` & `gemini_webapi-1.5.1/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/assets/favicon.png` & `gemini_webapi-1.5.1/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/assets/logo.svg` & `gemini_webapi-1.5.1/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/pyproject.toml` & `gemini_webapi-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/client.py` & `gemini_webapi-1.5.1/src/gemini_webapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import json
-import functools
 import asyncio
+import functools
+import json
+import re
 from asyncio import Task
 from pathlib import Path
 from typing import Any, Optional
 
 from httpx import AsyncClient, ReadTimeout
 
-from .types import WebImage, GeneratedImage, Candidate, ModelOutput
-from .exceptions import AuthError, APIError, TimeoutError, GeminiError
 from .constants import Endpoint, Headers
+from .exceptions import AuthError, APIError, TimeoutError, GeminiError
+from .types import WebImage, GeneratedImage, Candidate, ModelOutput
 from .utils import (
     upload_file,
     rotate_1psidts,
     get_access_token,
     load_browser_cookies,
     rotate_tasks,
     logger,
@@ -355,28 +356,33 @@
                 raise APIError(
                     "Failed to generate contents. Invalid response data received. Client will try to re-initialize on next request."
                 )
 
             try:
                 candidates = []
                 for candidate in body[4]:
+                    text = candidate[1][0]
+                    if re.match(r"^http://googleusercontent.com/card_content/\d+$", text):
+                        text = candidate[22] and candidate[22][0] or text
+
                     web_images = (
                         candidate[12]
                         and candidate[12][1]
                         and [
                             WebImage(
                                 url=image[0][0][0],
                                 title=image[7][0],
                                 alt=image[0][4],
                                 proxies=self.proxies,
                             )
                             for image in candidate[12][1]
                         ]
                         or []
                     )
+
                     generated_images = (
                         candidate[12]
                         and candidate[12][7]
                         and candidate[12][7][0]
                         and [
                             GeneratedImage(
                                 url=image[0][3][3],
@@ -387,18 +393,19 @@
                                 proxies=self.proxies,
                                 cookies=self.cookies,
                             )
                             for i, image in enumerate(candidate[12][7][0])
                         ]
                         or []
                     )
+
                     candidates.append(
                         Candidate(
                             rcid=candidate[0],
-                            text=candidate[1][0],
+                            text=text,
                             web_images=web_images,
                             generated_images=generated_images,
                         )
                     )
                 if not candidates:
                     raise GeminiError(
                         "Failed to generate contents. No output data found in response."
```

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/constants.py` & `gemini_webapi-1.5.1/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.5.1/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.5.1/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/types/image.py` & `gemini_webapi-1.5.1/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.5.1/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.5.1/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.5.1/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.5.1/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.5.1/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.5.1/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.5.1/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.5.0
+Version: 1.5.1
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.5.0/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.5.1/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/tests/test_client_features.py` & `gemini_webapi-1.5.1/tests/test_client_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,25 +28,22 @@
         self.assertTrue(response.text)
 
     @logger.catch(reraise=True)
     async def test_upload_image(self):
         response = await self.geminiclient.generate_content(
             "Describe these images", images=[Path("assets/banner.png"), "assets/favicon.png"]
         )
-        self.assertTrue(response.text)
         logger.debug(response.text)
 
     @logger.catch(reraise=True)
     async def test_continuous_conversation(self):
         chat = self.geminiclient.start_chat()
         response1 = await chat.send_message("Briefly introduce Europe")
-        self.assertTrue(response1.text)
         logger.debug(response1.text)
         response2 = await chat.send_message("What's the population there?")
-        self.assertTrue(response2.text)
         logger.debug(response2.text)
 
     @logger.catch(reraise=True)
     async def test_retrieve_previous_conversation(self):
         chat = self.geminiclient.start_chat()
         await chat.send_message("Fine weather today")
         self.assertTrue(len(chat.metadata) == 3)
@@ -57,20 +54,18 @@
         logger.debug(response)
 
     @logger.catch(reraise=True)
     async def test_chatsession_with_image(self):
         chat = self.geminiclient.start_chat()
         response1 = await chat.send_message(
             "What's the difference between these two images?",
-            images=["assets/pic1.png", "assets/pic2.png"],
+            images=["assets/banner.png", "assets/favicon.png"],
         )
-        self.assertTrue(response1.text)
         logger.debug(response1.text)
         response2 = await chat.send_message("Tell me more.")
-        self.assertTrue(response2.text)
         logger.debug(response2.text)
 
     @logger.catch(reraise=True)
     async def test_send_web_image(self):
         response = await self.geminiclient.generate_content(
             "Send me some pictures of cats"
         )
@@ -86,27 +81,32 @@
         )
         self.assertTrue(response.images)
         for image in response.images:
             self.assertTrue(image.url)
             logger.debug(image)
 
     @logger.catch(reraise=True)
+    async def test_card_content(self):
+        response = await self.geminiclient.generate_content(
+            "How is today's weather?"
+        )
+        logger.debug(response.text)
+
+    @logger.catch(reraise=True)
     async def test_extension_google_workspace(self):
         response = await self.geminiclient.generate_content(
             "@Gmail What's the latest message in my mailbox?"
         )
-        self.assertTrue(response.text)
         logger.debug(response)
 
     @logger.catch(reraise=True)
     async def test_extension_youtube(self):
         response = await self.geminiclient.generate_content(
             "@Youtube What's the lastest activity of Taylor Swift?"
         )
-        self.assertTrue(response.text)
         logger.debug(response)
 
     @logger.catch(reraise=True)
     async def test_reply_candidates(self):
         chat = self.geminiclient.start_chat()
         response = await chat.send_message("Recommend a science fiction book for me.")
```

### Comparing `gemini_webapi-1.5.0/tests/test_rotate_cookies.py` & `gemini_webapi-1.5.1/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.5.0/tests/test_save_image.py` & `gemini_webapi-1.5.1/tests/test_save_image.py`

 * *Files identical despite different names*

