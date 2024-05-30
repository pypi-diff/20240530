# Comparing `tmp/anipy_api-3.1.1.tar.gz` & `tmp/anipy_api-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.1.1.tar", max compression
+gzip compressed data, was "anipy_api-3.1.2.tar", max compression
```

## Comparing `anipy_api-3.1.1.tar` & `anipy_api-3.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      227 2024-05-29 11:08:11.630784 anipy_api-3.1.1/README.md
--rw-r--r--   0        0        0      825 2024-05-29 11:08:11.630784 anipy_api-3.1.1/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-29 11:08:11.630784 anipy_api-3.1.1/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5493 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11550 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/error.py
--rw-r--r--   0        0        0     8130 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2651 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0      183 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12198 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     8588 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/yugen_provider.py
--rw-r--r--   0        0        0      896 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 anipy_api-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-30 12:07:29.289708 anipy_api-3.1.2/README.md
+-rw-r--r--   0        0        0      825 2024-05-30 12:07:29.289708 anipy_api-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5493 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/error.py
+-rw-r--r--   0        0        0     8130 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2651 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0      183 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12198 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     8596 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/providers/yugen_provider.py
+-rw-r--r--   0        0        0      896 2024-05-30 12:07:29.289708 anipy_api-3.1.2/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 anipy_api-3.1.2/PKG-INFO
```

### Comparing `anipy_api-3.1.1/pyproject.toml` & `anipy_api-3.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.1.1"
+version = "3.1.2"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
```

### Comparing `anipy_api-3.1.1/src/anipy_api/anime.py` & `anipy_api-3.1.2/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/download.py` & `anipy_api-3.1.2/src/anipy_api/download.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/error.py` & `anipy_api-3.1.2/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/locallist.py` & `anipy_api-3.1.2/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/mal.py` & `anipy_api-3.1.2/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/base.py` & `anipy_api-3.1.2/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/player.py` & `anipy_api-3.1.2/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/players/mpv.py` & `anipy_api-3.1.2/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.1.2/src/anipy_api/player/players/mpv_control.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.1.2/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/player/players/vlc.py` & `anipy_api-3.1.2/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/__init__.py` & `anipy_api-3.1.2/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/base.py` & `anipy_api-3.1.2/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/filter.py` & `anipy_api-3.1.2/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/provider.py` & `anipy_api-3.1.2/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.1.2/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/providers/yugen_provider.py` & `anipy_api-3.1.2/src/anipy_api/provider/providers/yugen_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             "alternative_names": [],
         }
 
         soup = BeautifulSoup(result.text, "html.parser")
 
         name = soup.find("h1")
         if name is not None:
-            data_map["name"] = name.get_text()
+            data_map["name"] = name.get_text().strip()
 
         synopsis = soup.find("p", attrs={"class": "description"})
         if synopsis is not None:
             data_map["synopsis"] = synopsis.get_text("\n")
 
         image = soup.find("img", attrs={"class": "cover"})
         if image is not None:
```

### Comparing `anipy_api-3.1.1/src/anipy_api/provider/utils.py` & `anipy_api-3.1.2/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.1/PKG-INFO` & `anipy_api-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.1.1
+Version: 3.1.2
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

