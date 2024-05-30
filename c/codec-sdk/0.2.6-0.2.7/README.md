# Comparing `tmp/codec_sdk-0.2.6.tar.gz` & `tmp/codec_sdk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codec_sdk-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "codec_sdk-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `codec_sdk-0.2.6.tar` & `codec_sdk-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.6/.gitignore
--rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.6/.pypirc
--rw-r--r--   0        0        0      599 2024-04-03 18:51:17.775800 codec_sdk-0.2.6/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.6/LICENSE
--rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.6/Pipfile
--rw-r--r--   0        0        0     1339 2024-04-03 12:24:08.966117 codec_sdk-0.2.6/README.md
--rw-r--r--   0        0        0       95 2024-04-03 18:51:03.934471 codec_sdk-0.2.6/codec/__init__.py
--rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.6/codec/auth.py
--rw-r--r--   0        0        0     1060 2024-04-03 12:28:04.791143 codec_sdk-0.2.6/codec/client.py
--rw-r--r--   0        0        0     1297 2024-04-03 18:48:47.300372 codec_sdk-0.2.6/codec/constants.py
--rw-r--r--   0        0        0     1154 2024-03-31 16:38:04.420397 codec_sdk-0.2.6/codec/exceptions.py
--rw-r--r--   0        0        0      157 2024-04-02 18:49:59.803952 codec_sdk-0.2.6/codec/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.6/codec/resources/collections/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-02 18:32:08.559513 codec_sdk-0.2.6/codec/resources/collections/collections.py
--rw-r--r--   0        0        0      452 2024-04-03 12:26:14.996441 codec_sdk-0.2.6/codec/resources/collections/format.py
--rw-r--r--   0        0        0      240 2024-04-03 12:28:08.755135 codec_sdk-0.2.6/codec/resources/collections/types.py
--rw-r--r--   0        0        0       98 2024-03-31 16:53:09.176751 codec_sdk-0.2.6/codec/resources/logger.py
--rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.6/codec/resources/request.py
--rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.6/codec/resources/search/__init__.py
--rw-r--r--   0        0        0      604 2024-03-31 16:40:39.439653 codec_sdk-0.2.6/codec/resources/search/search.py
--rw-r--r--   0        0        0      273 2024-04-03 12:30:00.980022 codec_sdk-0.2.6/codec/resources/search/types.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.6/codec/resources/videos/__init__.py
--rw-r--r--   0        0        0      347 2024-04-03 12:26:46.601634 codec_sdk-0.2.6/codec/resources/videos/format.py
--rw-r--r--   0        0        0      468 2024-04-03 12:29:19.052679 codec_sdk-0.2.6/codec/resources/videos/types.py
--rw-r--r--   0        0        0     2852 2024-04-03 12:29:48.049822 codec_sdk-0.2.6/codec/resources/videos/videos.py
--rw-r--r--   0        0        0       51 2024-04-02 18:34:36.254380 codec_sdk-0.2.6/codec/resources/webhook/__init__.py
--rw-r--r--   0        0        0     1092 2024-04-02 18:49:57.471447 codec_sdk-0.2.6/codec/resources/webhook/webhook.py
--rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.6/codec/utils/__init__.py
--rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.6/codec/utils/file_utils.py
--rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.6/codec/utils/type_utils.py
--rw-r--r--   0        0        0      606 2024-03-31 16:16:51.826816 codec_sdk-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 codec_sdk-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.7/.gitignore
+-rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.7/.pypirc
+-rw-r--r--   0        0        0      599 2024-04-03 18:51:17.775800 codec_sdk-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.7/LICENSE
+-rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.7/Pipfile
+-rw-r--r--   0        0        0     1339 2024-04-03 12:24:08.966117 codec_sdk-0.2.7/README.md
+-rw-r--r--   0        0        0       95 2024-05-30 17:01:27.476893 codec_sdk-0.2.7/codec/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.7/codec/auth.py
+-rw-r--r--   0        0        0     1060 2024-04-03 12:28:04.791143 codec_sdk-0.2.7/codec/client.py
+-rw-r--r--   0        0        0     1297 2024-04-03 18:48:47.300372 codec_sdk-0.2.7/codec/constants.py
+-rw-r--r--   0        0        0     1154 2024-03-31 16:38:04.420397 codec_sdk-0.2.7/codec/exceptions.py
+-rw-r--r--   0        0        0      157 2024-04-02 18:49:59.803952 codec_sdk-0.2.7/codec/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.7/codec/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 18:32:08.559513 codec_sdk-0.2.7/codec/resources/collections/collections.py
+-rw-r--r--   0        0        0      452 2024-04-03 12:26:14.996441 codec_sdk-0.2.7/codec/resources/collections/format.py
+-rw-r--r--   0        0        0      240 2024-04-03 12:28:08.755135 codec_sdk-0.2.7/codec/resources/collections/types.py
+-rw-r--r--   0        0        0       98 2024-03-31 16:53:09.176751 codec_sdk-0.2.7/codec/resources/logger.py
+-rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.7/codec/resources/request.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.7/codec/resources/search/__init__.py
+-rw-r--r--   0        0        0      604 2024-03-31 16:40:39.439653 codec_sdk-0.2.7/codec/resources/search/search.py
+-rw-r--r--   0        0        0      273 2024-04-03 12:30:00.980022 codec_sdk-0.2.7/codec/resources/search/types.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.7/codec/resources/videos/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-03 12:26:46.601634 codec_sdk-0.2.7/codec/resources/videos/format.py
+-rw-r--r--   0        0        0      495 2024-05-30 17:00:37.005204 codec_sdk-0.2.7/codec/resources/videos/types.py
+-rw-r--r--   0        0        0     2852 2024-04-03 12:29:48.049822 codec_sdk-0.2.7/codec/resources/videos/videos.py
+-rw-r--r--   0        0        0       51 2024-04-02 18:34:36.254380 codec_sdk-0.2.7/codec/resources/webhook/__init__.py
+-rw-r--r--   0        0        0     1092 2024-04-02 18:49:57.471447 codec_sdk-0.2.7/codec/resources/webhook/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.7/codec/utils/__init__.py
+-rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.7/codec/utils/file_utils.py
+-rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.7/codec/utils/type_utils.py
+-rw-r--r--   0        0        0      606 2024-05-30 17:01:33.589222 codec_sdk-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 codec_sdk-0.2.7/PKG-INFO
```

### Comparing `codec_sdk-0.2.6/.gitignore` & `codec_sdk-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/CHANGELOG.md` & `codec_sdk-0.2.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/LICENSE` & `codec_sdk-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/README.md` & `codec_sdk-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/client.py` & `codec_sdk-0.2.7/codec/client.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/constants.py` & `codec_sdk-0.2.7/codec/constants.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/exceptions.py` & `codec_sdk-0.2.7/codec/exceptions.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/resources/collections/collections.py` & `codec_sdk-0.2.7/codec/resources/collections/collections.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/resources/request.py` & `codec_sdk-0.2.7/codec/resources/request.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/resources/search/search.py` & `codec_sdk-0.2.7/codec/resources/search/search.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/resources/videos/videos.py` & `codec_sdk-0.2.7/codec/resources/videos/videos.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/resources/webhook/webhook.py` & `codec_sdk-0.2.7/codec/resources/webhook/webhook.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/codec/utils/file_utils.py` & `codec_sdk-0.2.7/codec/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/pyproject.toml` & `codec_sdk-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.6/PKG-INFO` & `codec_sdk-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codec-sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python Library for the Codec API
 Author-email: Armada Labs Inc <contact@codec.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >=2.31.0
 Requires-Dist: supabase >=1.0.3
```

