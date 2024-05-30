# Comparing `tmp/rockai_cli_app-0.2.7.tar.gz` & `tmp/rockai_cli_app-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.7.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.8.tar", max compression
```

## Comparing `rockai_cli_app-0.2.7.tar` & `rockai_cli_app-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1181 2024-05-30 08:10:29.119571 rockai_cli_app-0.2.7/README.md
--rw-r--r--   0        0        0      717 2024-05-30 08:39:05.623736 rockai_cli_app-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     8044 2024-05-30 08:09:03.481852 rockai_cli_app-0.2.7/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.7/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.7/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    12294 2024-05-30 08:34:54.724275 rockai_cli_app-0.2.7/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     1351 2024-05-30 08:18:34.749394 rockai_cli_app-0.2.7/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      646 2024-05-30 08:22:44.453285 rockai_cli_app-0.2.7/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.7/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.7/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.7/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0     1297 2024-05-30 08:12:33.778287 rockai_cli_app-0.2.7/rockai_cli_app/rock.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.7/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.7/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.7/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.7/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.7/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.7/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.7/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.7/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.7/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      413 2024-05-30 07:37:18.396062 rockai_cli_app-0.2.7/rockai_cli_app/test.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1181 2024-05-30 08:10:29.119571 rockai_cli_app-0.2.8/README.md
+-rw-r--r--   0        0        0      717 2024-05-30 15:09:32.074528 rockai_cli_app-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     8044 2024-05-30 08:09:03.481852 rockai_cli_app-0.2.8/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.8/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.8/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12306 2024-05-30 15:09:13.092384 rockai_cli_app-0.2.8/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     1351 2024-05-30 08:18:34.749394 rockai_cli_app-0.2.8/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      646 2024-05-30 08:22:44.453285 rockai_cli_app-0.2.8/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.8/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.8/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.8/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0     1308 2024-05-30 15:07:44.762751 rockai_cli_app-0.2.8/rockai_cli_app/rock.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.8/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.8/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.8/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.8/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.8/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.8/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.8/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.8/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.8/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      413 2024-05-30 07:37:18.396062 rockai_cli_app-0.2.8/rockai_cli_app/test.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.8/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.7/README.md` & `rockai_cli_app-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/pyproject.toml` & `rockai_cli_app-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.7"
+version = "0.2.8"
 description = "Python SDK for RockAI.online"
 authors = ["RockAI <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.rock:app"
```

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/__init__.py` & `rockai_cli_app-0.2.8/rockai_cli_app/__init__.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.8/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.8/rockai_cli_app/docker/docker_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     if config_map['build']['python_requirements']:
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-metal')
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-macos')
         docker_list.append(add_run("pip install -r {} {}".format(config_map['build']['python_requirements'],"-i https://mirrors.aliyun.com/pypi/simple/")))
 
     docker_list.append(add_cmd("rock start"))
     docker_file_name = save_docker_file(docker_list)
-    subprocess.run(["docker", "build", "--platform", platform,"-t", tag,"-f {}".format(docker_file_name), "."])
+    subprocess.run(["docker", "build", "--platform", platform,"-t", tag,"-f {}".format(docker_file_name), Path.cwd() / ''])
     # subprocess.run(["docker", "run", "--rm", tag])
         
 
 
 def tf_compat_matrix():
     json_data = [{"tf_version": "tensorflow-2.16.1", "python": "3.9-3.12", "cuDNN": "8.9", "CUDA": "12.3"},{"tf_version": "tensorflow-2.15.0", "python": "3.9-3.11", "cuDNN": "8.9", "CUDA": "12.2"}, {"tf_version": "tensorflow-2.14.0", "python": "3.9-3.11", "cuDNN": "8.7", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.13.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.12.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.11.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.10.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.9.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.8.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.7.0", "python": "3.7-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.6.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.5.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.4.0", "python": "3.6-3.8", "cuDNN": "8.0", "CUDA": "11.0"}, {"tf_version": "tensorflow-2.3.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.2.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.1.0", "python": "2.7,", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.0.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.15.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.14.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.13.1", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.12.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.11.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.10.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.9.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.8.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.7.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.6.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.5.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.4.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.3.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.2.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.1.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.0.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}]
     return json_data
```

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.2.8/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.8/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.8/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/rock.py` & `rockai_cli_app-0.2.8/rockai_cli_app/rock.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 
 
 # @app.command()
 # def login():
 #     """
 #     Login using auth token
 #     """
-#     typer.echo("Login to Rock ai")
+#     typer.echo("Login to RockAI")
 
 
 @app.command()
 def init():
     file = open('rock.yaml', 'w')
     file.close()
     file = open('predict.py', 'w')
     file.close()
 
 
 
-@app.command()
+@app.command(name='build')
 def build():
     """
     Build the image
     """
     config_path: Path = Path.cwd() / "rock.yaml"
     if not config_path.is_file():
         raise Exception("rock.yaml config file doesn't exist in the current directory")
```

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.8/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.8/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.8/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.8/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.7/PKG-INFO` & `rockai_cli_app-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python SDK for RockAI.online
 Author: RockAI
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

