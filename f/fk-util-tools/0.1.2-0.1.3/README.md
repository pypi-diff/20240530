# Comparing `tmp/fk_util_tools-0.1.2.tar.gz` & `tmp/fk_util_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fk_util_tools-0.1.2.tar", last modified: Mon May  6 15:28:52 2024, max compression
+gzip compressed data, was "fk_util_tools-0.1.3.tar", last modified: Thu May 30 19:48:44 2024, max compression
```

## Comparing `fk_util_tools-0.1.2.tar` & `fk_util_tools-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_util_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-06 15:28:52.000000 fk_util_tools-0.1.2/fk_util_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 15:28:52.000000 fk_util_tools-0.1.2/fk_util_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:28:52.000000 fk_util_tools-0.1.2/fk_util_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 15:28:52.000000 fk_util_tools-0.1.2/fk_util_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 15:28:52.000000 fk_util_tools-0.1.2/fk_util_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/envs/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/envs/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/envs/aws/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/envs/aws/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/middlewares/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/django/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/middlewares/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/fastapi/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/middlewares/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/middlewares/flask/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/traces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/traces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/traces/datadog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/traces/datadog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/fk_utils/traces/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:47.000000 fk_util_tools-0.1.2/fk_utils/traces/opentelemetry/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-06 15:28:52.725163 fk_util_tools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 15:28:50.000000 fk_util_tools-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_util_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 19:48:44.000000 fk_util_tools-0.1.3/fk_util_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/envs/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/envs/aws/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.212690 fk_util_tools-0.1.3/fk_utils/middlewares/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/django/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/fastapi/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/middlewares/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/middlewares/flask/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/datadog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/datadog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/django/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/fastapi/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-30 19:48:39.000000 fk_util_tools-0.1.3/fk_utils/traces/opentelemetry/flask/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 19:48:44.216690 fk_util_tools-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-30 19:48:42.000000 fk_util_tools-0.1.3/setup.py
```

### Comparing `fk_util_tools-0.1.2/LICENSE` & `fk_util_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.2/fk_util_tools.egg-info/SOURCES.txt` & `fk_util_tools-0.1.3/fk_util_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,14 @@
 fk_utils/middlewares/django/handler.py
 fk_utils/middlewares/fastapi/__init__.py
 fk_utils/middlewares/fastapi/handler.py
 fk_utils/middlewares/flask/__init__.py
 fk_utils/middlewares/flask/handler.py
 fk_utils/traces/__init__.py
 fk_utils/traces/datadog/__init__.py
-fk_utils/traces/opentelemetry/__init__.py
+fk_utils/traces/opentelemetry/__init__.py
+fk_utils/traces/opentelemetry/django/__init__.py
+fk_utils/traces/opentelemetry/django/trace.py
+fk_utils/traces/opentelemetry/fastapi/__init__.py
+fk_utils/traces/opentelemetry/fastapi/trace.py
+fk_utils/traces/opentelemetry/flask/__init__.py
+fk_utils/traces/opentelemetry/flask/trace.py
```

### Comparing `fk_util_tools-0.1.2/fk_utils/config.py` & `fk_util_tools-0.1.3/fk_utils/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,7 +9,12 @@
         self.REPOSITORY = os.environ.get('REPOSITORY', 'msa_repository')
         self.TYPE_DEPLOY = os.environ.get('TYPE_DEPLOY', 'api')
 
         # AWS
         self.AWS_PROFILE_NAME = os.environ.get('AWS_PROFILE_NAME', 'default')
         self.AWS_REGION_NAME = os.environ.get('AWS_REGION_NAME', 'us-east-1')
         self.SECRET_NAME = os.environ.get('SECRET_NAME', 'api/testing/ms-communicator')
+
+        # Opentelemtry
+        self.OTLP_HOST = os.environ.get('OTLP_HOST', 'localhost')
+        self.OTLP_PORT = os.environ.get('OTLP_PORT', '0000')
+        self.OTLP_NAME = os.environ.get('OTLP_NAME', 'ms-localhost')
```

### Comparing `fk_util_tools-0.1.2/fk_utils/envs/aws/parameters.py` & `fk_util_tools-0.1.3/fk_utils/envs/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.2/fk_utils/envs/aws/secrets.py` & `fk_util_tools-0.1.3/fk_utils/envs/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.2/setup.cfg` & `fk_util_tools-0.1.3/setup.cfg`

 * *Files identical despite different names*

