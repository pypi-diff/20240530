# Comparing `tmp/dwave_sona_core-1.3.1.tar.gz` & `tmp/dwave_sona_core-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave_sona_core-1.3.1.tar", max compression
+gzip compressed data, was "dwave_sona_core-1.3.2.tar", max compression
```

## Comparing `dwave_sona_core-1.3.1.tar` & `dwave_sona_core-1.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1085 2024-04-29 09:40:42.005779 dwave_sona_core-1.3.1/LICENSE
--rw-r--r--   0        0        0     2382 2024-04-29 09:40:42.017779 dwave_sona_core-1.3.1/README.md
--rw-r--r--   0        0        0      965 2024-05-16 09:37:45.071488 dwave_sona_core-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      308 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/__init__.py
--rw-r--r--   0        0        0       59 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/__main__.py
--rw-r--r--   0        0        0     1157 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/commands.py
--rw-r--r--   0        0        0       98 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/exceptions.py
--rw-r--r--   0        0        0     4100 2024-05-07 11:17:04.856934 dwave_sona_core-1.3.1/sona/core/inferencer.py
--rw-r--r--   0        0        0      155 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/messages/__init__.py
--rw-r--r--   0        0        0      364 2024-05-06 09:59:41.001325 dwave_sona_core-1.3.1/sona/core/messages/base.py
--rw-r--r--   0        0        0     1892 2024-05-06 10:18:17.921108 dwave_sona_core-1.3.1/sona/core/messages/context.py
--rw-r--r--   0        0        0     1283 2024-05-08 02:52:18.180538 dwave_sona_core-1.3.1/sona/core/messages/file.py
--rw-r--r--   0        0        0     1422 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/messages/job.py
--rw-r--r--   0        0        0      353 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/messages/result.py
--rw-r--r--   0        0        0      797 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/messages/state.py
--rw-r--r--   0        0        0      265 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/middlewares/__init__.py
--rw-r--r--   0        0        0     1213 2024-05-07 08:30:52.602643 dwave_sona_core-1.3.1/sona/core/middlewares/base.py
--rw-r--r--   0        0        0     6722 2024-05-16 09:33:37.576520 dwave_sona_core-1.3.1/sona/core/middlewares/supervisors.py
--rw-r--r--   0        0        0     2410 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/middlewares/tracer.py
--rw-r--r--   0        0        0      242 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/storages/__init__.py
--rw-r--r--   0        0        0      888 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/storages/azureblob.py
--rw-r--r--   0        0        0     2751 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/storages/base.py
--rw-r--r--   0        0        0      578 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.1/sona/core/storages/filters/audio.py
--rw-r--r--   0        0        0      629 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/local.py
--rw-r--r--   0        0        0      865 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/s3.py
--rw-r--r--   0        0        0      187 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/__init__.py
--rw-r--r--   0        0        0     1146 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/azureblob.py
--rw-r--r--   0        0        0      294 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/base.py
--rw-r--r--   0        0        0     1246 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/gdrive.py
--rw-r--r--   0        0        0      796 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/http.py
--rw-r--r--   0        0        0      682 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/local.py
--rw-r--r--   0        0        0     1168 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/storages/sources/s3.py
--rw-r--r--   0        0        0      996 2024-04-30 02:20:52.580444 dwave_sona_core-1.3.1/sona/core/storages/sources/youtube.py
--rw-r--r--   0        0        0     2127 2024-05-07 06:54:34.802357 dwave_sona_core-1.3.1/sona/core/stream/inferencer.py
--rw-r--r--   0        0        0       61 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/stream/messages/__init__.py
--rw-r--r--   0        0        0      304 2024-05-07 06:57:28.323905 dwave_sona_core-1.3.1/sona/core/stream/messages/context.py
--rw-r--r--   0        0        0     1205 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/stream/messages/streamdata.py
--rw-r--r--   0        0        0     1029 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/core/stream/parsers/audio.py
--rw-r--r--   0        0        0     2168 2024-05-16 03:54:31.891648 dwave_sona_core-1.3.1/sona/settings.py
--rw-r--r--   0        0        0     2042 2024-05-08 02:50:46.586961 dwave_sona_core-1.3.1/sona/utils/common.py
--rw-r--r--   0        0        0      215 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/web/commands.py
--rw-r--r--   0        0        0       74 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/web/messages/__init__.py
--rw-r--r--   0        0        0      117 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/web/messages/requests.py
--rw-r--r--   0        0        0      172 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/web/messages/responses.py
--rw-r--r--   0        0        0     3059 2024-05-07 08:44:44.758714 dwave_sona_core-1.3.1/sona/web/rpc/handlers.py
--rw-r--r--   0        0        0      995 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/web/rpc/tracks.py
--rw-r--r--   0        0        0     5083 2024-05-16 09:36:55.498832 dwave_sona_core-1.3.1/sona/web/server.py
--rw-r--r--   0        0        0     9838 2024-05-07 08:23:11.503489 dwave_sona_core-1.3.1/sona/web/static/client.js
--rw-r--r--   0        0        0     3714 2024-05-07 08:22:34.671622 dwave_sona_core-1.3.1/sona/web/static/webrtc.html
--rw-r--r--   0        0        0        0 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/__init__.py
--rw-r--r--   0        0        0      948 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/commands.py
--rw-r--r--   0        0        0      560 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/consumers/__init__.py
--rw-r--r--   0        0        0      223 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/consumers/base.py
--rw-r--r--   0        0        0     1112 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/consumers/kafka.py
--rw-r--r--   0        0        0     1299 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/consumers/redis.py
--rw-r--r--   0        0        0     1021 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/consumers/sqs.py
--rw-r--r--   0        0        0      560 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/producers/__init__.py
--rw-r--r--   0        0        0      131 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/producers/base.py
--rw-r--r--   0        0        0      651 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/producers/kafka.py
--rw-r--r--   0        0        0      387 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/producers/redis.py
--rw-r--r--   0        0        0      387 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.1/sona/worker/producers/sqs.py
--rw-r--r--   0        0        0     2834 2024-04-30 02:20:52.580444 dwave_sona_core-1.3.1/sona/worker/workers.py
--rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 dwave_sona_core-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-29 09:40:42.005779 dwave_sona_core-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2382 2024-05-30 06:10:24.292775 dwave_sona_core-1.3.2/README.md
+-rw-r--r--   0        0        0      965 2024-05-30 06:14:45.638813 dwave_sona_core-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/__main__.py
+-rw-r--r--   0        0        0     1157 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/commands.py
+-rw-r--r--   0        0        0       98 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/exceptions.py
+-rw-r--r--   0        0        0     4100 2024-05-07 11:17:04.856934 dwave_sona_core-1.3.2/sona/core/inferencer.py
+-rw-r--r--   0        0        0      155 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/messages/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-06 09:59:41.001325 dwave_sona_core-1.3.2/sona/core/messages/base.py
+-rw-r--r--   0        0        0     1892 2024-05-06 10:18:17.921108 dwave_sona_core-1.3.2/sona/core/messages/context.py
+-rw-r--r--   0        0        0     1283 2024-05-08 02:52:18.180538 dwave_sona_core-1.3.2/sona/core/messages/file.py
+-rw-r--r--   0        0        0     1422 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/messages/job.py
+-rw-r--r--   0        0        0      353 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/messages/result.py
+-rw-r--r--   0        0        0      797 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/messages/state.py
+-rw-r--r--   0        0        0      265 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/core/middlewares/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-16 16:21:57.726503 dwave_sona_core-1.3.2/sona/core/middlewares/base.py
+-rw-r--r--   0        0        0     6722 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/core/middlewares/supervisors.py
+-rw-r--r--   0        0        0     2410 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/core/middlewares/tracer.py
+-rw-r--r--   0        0        0      242 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/storages/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/storages/azureblob.py
+-rw-r--r--   0        0        0     2751 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/storages/base.py
+-rw-r--r--   0        0        0      578 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.2/sona/core/storages/filters/audio.py
+-rw-r--r--   0        0        0      629 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/local.py
+-rw-r--r--   0        0        0      865 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/s3.py
+-rw-r--r--   0        0        0      187 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/azureblob.py
+-rw-r--r--   0        0        0      294 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/base.py
+-rw-r--r--   0        0        0     1246 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/gdrive.py
+-rw-r--r--   0        0        0      796 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/http.py
+-rw-r--r--   0        0        0      682 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/local.py
+-rw-r--r--   0        0        0     1168 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.2/sona/core/storages/sources/s3.py
+-rw-r--r--   0        0        0      996 2024-04-30 02:20:52.580444 dwave_sona_core-1.3.2/sona/core/storages/sources/youtube.py
+-rw-r--r--   0        0        0     2127 2024-05-30 06:10:17.956722 dwave_sona_core-1.3.2/sona/core/stream/inferencer.py
+-rw-r--r--   0        0        0       61 2024-05-30 06:10:17.956722 dwave_sona_core-1.3.2/sona/core/stream/messages/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-30 06:10:17.956722 dwave_sona_core-1.3.2/sona/core/stream/messages/context.py
+-rw-r--r--   0        0        0     1205 2024-05-30 06:10:17.956722 dwave_sona_core-1.3.2/sona/core/stream/messages/streamdata.py
+-rw-r--r--   0        0        0     1029 2024-05-30 06:10:17.956722 dwave_sona_core-1.3.2/sona/core/stream/parsers/audio.py
+-rw-r--r--   0        0        0     2168 2024-05-16 03:54:31.891648 dwave_sona_core-1.3.2/sona/settings.py
+-rw-r--r--   0        0        0     2042 2024-05-08 02:50:46.586961 dwave_sona_core-1.3.2/sona/utils/common.py
+-rw-r--r--   0        0        0      215 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/commands.py
+-rw-r--r--   0        0        0       74 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/messages/__init__.py
+-rw-r--r--   0        0        0      117 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/messages/requests.py
+-rw-r--r--   0        0        0      172 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/messages/responses.py
+-rw-r--r--   0        0        0     3446 2024-05-30 06:12:23.405739 dwave_sona_core-1.3.2/sona/web/rpc/handlers.py
+-rw-r--r--   0        0        0      995 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/rpc/tracks.py
+-rw-r--r--   0        0        0     5083 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/server.py
+-rw-r--r--   0        0        0     9838 2024-05-30 06:10:24.296775 dwave_sona_core-1.3.2/sona/web/static/client.js
+-rw-r--r--   0        0        0     3714 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/web/static/webrtc.html
+-rw-r--r--   0        0        0        0 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/__init__.py
+-rw-r--r--   0        0        0      948 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/commands.py
+-rw-r--r--   0        0        0      560 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/consumers/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/consumers/base.py
+-rw-r--r--   0        0        0     1112 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/consumers/kafka.py
+-rw-r--r--   0        0        0     1299 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/consumers/redis.py
+-rw-r--r--   0        0        0     1021 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/consumers/sqs.py
+-rw-r--r--   0        0        0      560 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/producers/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/producers/base.py
+-rw-r--r--   0        0        0      651 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/producers/kafka.py
+-rw-r--r--   0        0        0      387 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/producers/redis.py
+-rw-r--r--   0        0        0      387 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/producers/sqs.py
+-rw-r--r--   0        0        0     2834 2024-05-30 06:10:24.300775 dwave_sona_core-1.3.2/sona/worker/workers.py
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 dwave_sona_core-1.3.2/PKG-INFO
```

### Comparing `dwave_sona_core-1.3.1/LICENSE` & `dwave_sona_core-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/README.md` & `dwave_sona_core-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/pyproject.toml` & `dwave_sona_core-1.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwave-sona-core"
-version = "1.3.1"
+version = "1.3.2"
 description = ""
 authors = ["dwave-dev"]
 license = ""
 readme = "README.md"
 packages = [{include = "sona"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dwave_sona_core-1.3.1/sona/core/commands.py` & `dwave_sona_core-1.3.2/sona/core/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/inferencer.py` & `dwave_sona_core-1.3.2/sona/core/inferencer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/messages/context.py` & `dwave_sona_core-1.3.2/sona/core/messages/context.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/messages/file.py` & `dwave_sona_core-1.3.2/sona/core/messages/file.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/messages/job.py` & `dwave_sona_core-1.3.2/sona/core/messages/job.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/messages/state.py` & `dwave_sona_core-1.3.2/sona/core/messages/state.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/middlewares/base.py` & `dwave_sona_core-1.3.2/sona/core/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/middlewares/supervisors.py` & `dwave_sona_core-1.3.2/sona/core/middlewares/supervisors.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/middlewares/tracer.py` & `dwave_sona_core-1.3.2/sona/core/middlewares/tracer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/azureblob.py` & `dwave_sona_core-1.3.2/sona/core/storages/azureblob.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/base.py` & `dwave_sona_core-1.3.2/sona/core/storages/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/filters/audio.py` & `dwave_sona_core-1.3.2/sona/core/storages/filters/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/local.py` & `dwave_sona_core-1.3.2/sona/core/storages/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/s3.py` & `dwave_sona_core-1.3.2/sona/core/storages/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/azureblob.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/azureblob.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/gdrive.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/gdrive.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/http.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/http.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/local.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/s3.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/storages/sources/youtube.py` & `dwave_sona_core-1.3.2/sona/core/storages/sources/youtube.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/stream/inferencer.py` & `dwave_sona_core-1.3.2/sona/core/stream/inferencer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/stream/messages/streamdata.py` & `dwave_sona_core-1.3.2/sona/core/stream/messages/streamdata.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/core/stream/parsers/audio.py` & `dwave_sona_core-1.3.2/sona/core/stream/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/settings.py` & `dwave_sona_core-1.3.2/sona/settings.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/utils/common.py` & `dwave_sona_core-1.3.2/sona/utils/common.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/web/rpc/tracks.py` & `dwave_sona_core-1.3.2/sona/web/rpc/tracks.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/web/server.py` & `dwave_sona_core-1.3.2/sona/web/server.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/web/static/client.js` & `dwave_sona_core-1.3.2/sona/web/static/client.js`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/web/static/webrtc.html` & `dwave_sona_core-1.3.2/sona/web/static/webrtc.html`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/commands.py` & `dwave_sona_core-1.3.2/sona/worker/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/consumers/__init__.py` & `dwave_sona_core-1.3.2/sona/worker/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/consumers/kafka.py` & `dwave_sona_core-1.3.2/sona/worker/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/consumers/redis.py` & `dwave_sona_core-1.3.2/sona/worker/consumers/redis.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/consumers/sqs.py` & `dwave_sona_core-1.3.2/sona/worker/consumers/sqs.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/producers/__init__.py` & `dwave_sona_core-1.3.2/sona/worker/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/producers/kafka.py` & `dwave_sona_core-1.3.2/sona/worker/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/sona/worker/workers.py` & `dwave_sona_core-1.3.2/sona/worker/workers.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.3.1/PKG-INFO` & `dwave_sona_core-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-sona-core
-Version: 1.3.1
+Version: 1.3.2
 Summary: 
 Author: dwave-dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

