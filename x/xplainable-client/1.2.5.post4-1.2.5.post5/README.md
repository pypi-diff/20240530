# Comparing `tmp/xplainable_client-1.2.5.post4.tar.gz` & `tmp/xplainable_client-1.2.5.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.5.post4.tar", last modified: Wed May 29 13:06:43 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.5.post5.tar", last modified: Wed May 29 13:13:00 2024, max compression
```

## Comparing `xplainable_client-1.2.5.post4.tar` & `xplainable_client-1.2.5.post5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.476033 xplainable_client-1.2.5.post4/
--rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.5.post4/.gitignore
--rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post4/LICENSE
--rw-rw-rw-   0        0        0    45260 2024-05-29 13:06:43.475033 xplainable_client-1.2.5.post4/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post4/README.md
--rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.5.post4/_build.py
--rw-rw-rw-   0        0        0       29 2024-05-29 13:06:39.000000 xplainable_client-1.2.5.post4/_version.py
--rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post4/config.py
--rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/docker-compose.yaml
--rw-rw-rw-   0        0        0      783 2024-05-29 13:06:39.000000 xplainable_client-1.2.5.post4/pyproject.toml
--rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.5.post4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 13:06:43.476033 xplainable_client-1.2.5.post4/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-05-29 13:06:39.000000 xplainable_client-1.2.5.post4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.449033 xplainable_client-1.2.5.post4/tests/
--rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/tests/nanoid.sql
--rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/tests/prod-db.sql
--rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/tests/test_model.py
--rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/tests/test_test.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.450533 xplainable_client-1.2.5.post4/thebadboycorner/
--rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.5.post4/thebadboycorner/clf_model_test_jason.py
--rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.5.post4/thebadboycorner/test.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.452033 xplainable_client-1.2.5.post4/xplainable_client/
--rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.5.post4/xplainable_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.467033 xplainable_client-1.2.5.post4/xplainable_client/client/
--rw-rw-rw-   0        0        0     1034 2024-05-29 08:46:14.000000 xplainable_client-1.2.5.post4/xplainable_client/client/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_client_cog_base.py
--rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_collections.py
--rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_datasets.py
--rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_deployments.py
--rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_gpt.py
--rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_inference.py
--rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_misc.py
--rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_models.py
--rw-rw-rw-   0        0        0    10934 2024-05-28 01:15:50.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_preprocessing.py
--rw-rw-rw-   0        0        0     4418 2024-05-29 13:06:22.000000 xplainable_client-1.2.5.post4/xplainable_client/client/_session.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.472534 xplainable_client-1.2.5.post4/xplainable_client/client/utils/
--rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/encoders.py
--rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/helpers.py
--rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/metrics.py
--rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/model_parsers.py
--rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post4/xplainable_client/client/utils/scanner.py
--rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post4/xplainable_client/pytest.ini
-drwxrwxrwx   0        0        0        0 2024-05-29 13:06:43.473533 xplainable_client-1.2.5.post4/xplainable_client.egg-info/
--rw-rw-rw-   0        0        0    45260 2024-05-29 13:06:43.000000 xplainable_client-1.2.5.post4/xplainable_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-05-29 13:06:43.000000 xplainable_client-1.2.5.post4/xplainable_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:06:43.000000 xplainable_client-1.2.5.post4/xplainable_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-29 13:06:43.000000 xplainable_client-1.2.5.post4/xplainable_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-05-29 13:06:43.000000 xplainable_client-1.2.5.post4/xplainable_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.658244 xplainable_client-1.2.5.post5/
+-rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.5.post5/.gitignore
+-rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post5/LICENSE
+-rw-rw-rw-   0        0        0    45260 2024-05-29 13:13:00.657243 xplainable_client-1.2.5.post5/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post5/README.md
+-rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.5.post5/_build.py
+-rw-rw-rw-   0        0        0       29 2024-05-29 13:12:51.000000 xplainable_client-1.2.5.post5/_version.py
+-rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post5/config.py
+-rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/docker-compose.yaml
+-rw-rw-rw-   0        0        0      783 2024-05-29 13:12:51.000000 xplainable_client-1.2.5.post5/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.5.post5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:13:00.658244 xplainable_client-1.2.5.post5/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-05-29 13:12:51.000000 xplainable_client-1.2.5.post5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.632743 xplainable_client-1.2.5.post5/tests/
+-rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/tests/nanoid.sql
+-rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/tests/prod-db.sql
+-rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/tests/test_model.py
+-rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/tests/test_test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.634244 xplainable_client-1.2.5.post5/thebadboycorner/
+-rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.5.post5/thebadboycorner/clf_model_test_jason.py
+-rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.5.post5/thebadboycorner/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.635743 xplainable_client-1.2.5.post5/xplainable_client/
+-rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.5.post5/xplainable_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.649243 xplainable_client-1.2.5.post5/xplainable_client/client/
+-rw-rw-rw-   0        0        0     1034 2024-05-29 08:46:14.000000 xplainable_client-1.2.5.post5/xplainable_client/client/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_client_cog_base.py
+-rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_collections.py
+-rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_datasets.py
+-rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_deployments.py
+-rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_gpt.py
+-rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_inference.py
+-rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_misc.py
+-rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_models.py
+-rw-rw-rw-   0        0        0    10950 2024-05-29 13:11:19.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_preprocessing.py
+-rw-rw-rw-   0        0        0     4418 2024-05-29 13:06:22.000000 xplainable_client-1.2.5.post5/xplainable_client/client/_session.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.655243 xplainable_client-1.2.5.post5/xplainable_client/client/utils/
+-rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/encoders.py
+-rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/helpers.py
+-rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/metrics.py
+-rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/model_parsers.py
+-rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post5/xplainable_client/client/utils/scanner.py
+-rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post5/xplainable_client/pytest.ini
+drwxrwxrwx   0        0        0        0 2024-05-29 13:13:00.656245 xplainable_client-1.2.5.post5/xplainable_client.egg-info/
+-rw-rw-rw-   0        0        0    45260 2024-05-29 13:13:00.000000 xplainable_client-1.2.5.post5/xplainable_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2024-05-29 13:13:00.000000 xplainable_client-1.2.5.post5/xplainable_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:13:00.000000 xplainable_client-1.2.5.post5/xplainable_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-29 13:13:00.000000 xplainable_client-1.2.5.post5/xplainable_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2024-05-29 13:13:00.000000 xplainable_client-1.2.5.post5/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.5.post4/.gitignore` & `xplainable_client-1.2.5.post5/.gitignore`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/LICENSE` & `xplainable_client-1.2.5.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/PKG-INFO` & `xplainable_client-1.2.5.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.5.post4
+Version: 1.2.5.post5
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.5.post4/README.md` & `xplainable_client-1.2.5.post5/README.md`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/_build.py` & `xplainable_client-1.2.5.post5/_build.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/pyproject.toml` & `xplainable_client-1.2.5.post5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.5.post4"
+version = "1.2.5.post5"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `xplainable_client-1.2.5.post4/tests/nanoid.sql` & `xplainable_client-1.2.5.post5/tests/nanoid.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/tests/prod-db.sql` & `xplainable_client-1.2.5.post5/tests/prod-db.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/thebadboycorner/clf_model_test_jason.py` & `xplainable_client-1.2.5.post5/thebadboycorner/clf_model_test_jason.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/__init__.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_collections.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_collections.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_datasets.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_deployments.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_deployments.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_gpt.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_inference.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_inference.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_misc.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_misc.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_models.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_models.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_preprocessing.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             if df is not None:
                 after = delta_gen.__next__()
                 delta = get_df_delta(before.copy(), after.copy())
                 deltas.append(delta)
                 before = after.copy()
         # Get current versions
         versions = {
-            "xplainable_version": self.xplainable_version,
-            "python_version": self.python_version
+            "xplainable_version": self.session.xplainable_version,
+            "python_version": self.session.python_version
         }
         # Create payload
         payload = {
             "stages": stages,
             "deltas": deltas,
             "versions": versions
         }
```

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/_session.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/_session.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/utils/encoders.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/utils/helpers.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/utils/metrics.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/utils/model_parsers.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client/client/utils/scanner.py` & `xplainable_client-1.2.5.post5/xplainable_client/client/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5.post4/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.5.post5/xplainable_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.5.post4
+Version: 1.2.5.post5
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.5.post4/xplainable_client.egg-info/SOURCES.txt` & `xplainable_client-1.2.5.post5/xplainable_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

