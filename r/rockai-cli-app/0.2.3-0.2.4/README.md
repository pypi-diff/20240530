# Comparing `tmp/rockai_cli_app-0.2.3.tar.gz` & `tmp/rockai_cli_app-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.3.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.4.tar", max compression
```

## Comparing `rockai_cli_app-0.2.3.tar` & `rockai_cli_app-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0      244 2024-05-29 02:21:58.351513 rockai_cli_app-0.2.3/README.md
--rw-r--r--   0        0        0      715 2024-05-30 02:52:59.103217 rockai_cli_app-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 02:51:08.574355 rockai_cli_app-0.2.3/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     7769 2024-05-30 02:50:41.507845 rockai_cli_app-0.2.3/rockai_cli_app/client.py
--rw-r--r--   0        0        0       36 2024-05-16 02:40:27.277757 rockai_cli_app-0.2.3/rockai_cli_app/constant.py
--rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.3/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.3/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.3/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.3/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.3/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.3/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.3/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.3/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.3/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.3/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.3/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.3/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.3/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.3/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.3/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.3/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.3/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.3/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      393 2024-05-29 03:28:45.579316 rockai_cli_app-0.2.3/rockai_cli_app/test.py
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      244 2024-05-29 02:21:58.351513 rockai_cli_app-0.2.4/README.md
+-rw-r--r--   0        0        0      715 2024-05-30 04:44:30.520167 rockai_cli_app-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7769 2024-05-30 04:43:44.830882 rockai_cli_app-0.2.4/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-16 02:40:27.277757 rockai_cli_app-0.2.4/rockai_cli_app/constant.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.4/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.4/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.4/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.4/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.4/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.4/rockai_cli_app/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.4/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.4/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.4/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.4/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.4/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.4/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.4/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.4/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.4/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.4/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.4/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.4/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      393 2024-05-29 03:28:45.579316 rockai_cli_app-0.2.4/rockai_cli_app/test.py
+-rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.4/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.3/pyproject.toml` & `rockai_cli_app-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.3"
+version = "0.2.4"
 description = "For inference and training"
 authors = ["RockAI <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
```

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/client.py` & `rockai_cli_app-0.2.4/rockai_cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.4/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.4/rockai_cli_app/docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.2.4/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.4/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/main.py` & `rockai_cli_app-0.2.4/rockai_cli_app/main.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.4/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.4/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.4/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.4/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.4/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.3/PKG-INFO` & `rockai_cli_app-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.2.3
+Version: 0.2.4
 Summary: For inference and training
 Author: RockAI
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

