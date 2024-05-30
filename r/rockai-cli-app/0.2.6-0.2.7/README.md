# Comparing `tmp/rockai_cli_app-0.2.6.tar.gz` & `tmp/rockai_cli_app-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.6.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.7.tar", max compression
```

## Comparing `rockai_cli_app-0.2.6.tar` & `rockai_cli_app-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1181 2024-05-30 08:10:29.119571 rockai_cli_app-0.2.6/README.md
--rw-r--r--   0        0        0      717 2024-05-30 08:35:13.465910 rockai_cli_app-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     8044 2024-05-30 08:09:03.481852 rockai_cli_app-0.2.6/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.6/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.6/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    12294 2024-05-30 08:34:54.724275 rockai_cli_app-0.2.6/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     1351 2024-05-30 08:18:34.749394 rockai_cli_app-0.2.6/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      646 2024-05-30 08:22:44.453285 rockai_cli_app-0.2.6/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.6/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.6/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.6/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0     1297 2024-05-30 08:12:33.778287 rockai_cli_app-0.2.6/rockai_cli_app/rock.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.6/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.6/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.6/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.6/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.6/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.6/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.6/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.6/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.6/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      413 2024-05-30 07:37:18.396062 rockai_cli_app-0.2.6/rockai_cli_app/test.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1181 2024-05-30 08:10:29.119571 rockai_cli_app-0.2.7/README.md
+-rw-r--r--   0        0        0      717 2024-05-30 08:39:05.623736 rockai_cli_app-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     8044 2024-05-30 08:09:03.481852 rockai_cli_app-0.2.7/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.7/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.7/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12294 2024-05-30 08:34:54.724275 rockai_cli_app-0.2.7/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     1351 2024-05-30 08:18:34.749394 rockai_cli_app-0.2.7/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      646 2024-05-30 08:22:44.453285 rockai_cli_app-0.2.7/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.7/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.7/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.7/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0     1297 2024-05-30 08:12:33.778287 rockai_cli_app-0.2.7/rockai_cli_app/rock.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.7/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.7/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.7/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.7/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.7/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.7/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.7/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.7/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.7/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      413 2024-05-30 07:37:18.396062 rockai_cli_app-0.2.7/rockai_cli_app/test.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.7/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.6/README.md` & `rockai_cli_app-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/pyproject.toml` & `rockai_cli_app-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.6"
+version = "0.2.7"
 description = "Python SDK for RockAI.online"
 authors = ["RockAI <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
-rock = "rockai_cli_app.main:app"
+rock = "rockai_cli_app.rock:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
 fastapi = "^0.109.2"
 uvicorn = {extras = ["standard"], version = "^0.27.0.post1"}
 requests = "^2.31.0"
```

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/__init__.py` & `rockai_cli_app-0.2.7/rockai_cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.7/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.7/rockai_cli_app/docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.2.7/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.7/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.7/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/rock.py` & `rockai_cli_app-0.2.7/rockai_cli_app/rock.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.7/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.7/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.7/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.7/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.6/PKG-INFO` & `rockai_cli_app-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python SDK for RockAI.online
 Author: RockAI
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

