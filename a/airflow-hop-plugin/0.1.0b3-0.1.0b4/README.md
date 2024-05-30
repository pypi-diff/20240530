# Comparing `tmp/airflow-hop-plugin-0.1.0b3.tar.gz` & `tmp/airflow_hop_plugin-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-hop-plugin-0.1.0b3.tar", last modified: Mon Jan 15 15:00:20 2024, max compression
+gzip compressed data, was "airflow_hop_plugin-0.1.0b4.tar", last modified: Thu May 30 07:50:16 2024, max compression
```

## Comparing `airflow-hop-plugin-0.1.0b3.tar` & `airflow_hop_plugin-0.1.0b4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:00:20.961517 airflow-hop-plugin-0.1.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-01-15 15:00:20.961517 airflow-hop-plugin-0.1.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:00:20.961517 airflow-hop-plugin-0.1.0b3/airflow_hop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/airflow_hop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/airflow_hop/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/airflow_hop/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/airflow_hop/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/airflow_hop/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 15:00:20.961517 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-15 15:00:20.000000 airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 15:00:20.961517 airflow-hop-plugin-0.1.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-15 14:59:27.000000 airflow-hop-plugin-0.1.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:16.028611 airflow_hop_plugin-0.1.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-30 07:50:16.024611 airflow_hop_plugin-0.1.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:16.024611 airflow_hop_plugin-0.1.0b4/airflow_hop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/airflow_hop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/airflow_hop/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/airflow_hop/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/airflow_hop/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/airflow_hop/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:16.024611 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:50:15.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 07:50:16.000000 airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:50:16.028611 airflow_hop_plugin-0.1.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-30 07:49:28.000000 airflow_hop_plugin-0.1.0b4/setup.py
```

### Comparing `airflow-hop-plugin-0.1.0b3/LICENSE` & `airflow_hop_plugin-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-hop-plugin-0.1.0b3/PKG-INFO` & `airflow_hop_plugin-0.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-hop-plugin
-Version: 0.1.0b3
+Version: 0.1.0b4
 Home-page: https://github.com/damavis/airflow-hop-plugin
 Author: Damavis
 Author-email: info@damavis.com
 License: Apache 2.0
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
```

### Comparing `airflow-hop-plugin-0.1.0b3/README.md` & `airflow_hop_plugin-0.1.0b4/README.md`

 * *Files identical despite different names*

### Comparing `airflow-hop-plugin-0.1.0b3/airflow_hop/hooks.py` & `airflow_hop_plugin-0.1.0b4/airflow_hop/hooks.py`

 * *Files identical despite different names*

### Comparing `airflow-hop-plugin-0.1.0b3/airflow_hop/operators.py` & `airflow_hop_plugin-0.1.0b4/airflow_hop/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,22 @@
 
     def __init__(self,
                  workflow,
                  project_name,
                  log_level,
                  *args,
                  environment=None,
-                 params=None,
+                 hop_params=None,
                  hop_conn_id='hop_default',
                  **kwargs):
         super().__init__(*args, **kwargs)
         self.workflow = workflow
         self.project_name = project_name
         self.log_level = log_level
-        self.task_params = params
+        self.task_params = hop_params
         self.hop_conn_id = hop_conn_id
         self.environment = environment
 
     def __get_hop_client(self):
         return HopHook(
                 self.project_name,
                 self.environment,
@@ -116,24 +116,24 @@
     def __init__(self,
                  pipeline,
                  pipe_config,
                  project_name,
                  log_level,
                  *args,
                  environment=None,
-                 params=None,
+                 hop_params=None,
                  hop_conn_id='hop_default',
                  **kwargs):
         super().__init__(*args, **kwargs)
         self.pipeline = pipeline
         self.pipe_config = pipe_config
         self.project_name = project_name
         self.log_level = log_level
         self.hop_conn_id = hop_conn_id
-        self.task_params = params
+        self.task_params = hop_params
         self.environment = environment
 
     def __get_hop_client(self):
         return HopHook(
                 self.project_name,
                 self.environment,
                 self.hop_conn_id,
```

### Comparing `airflow-hop-plugin-0.1.0b3/airflow_hop/plugin.py` & `airflow_hop_plugin-0.1.0b4/airflow_hop/plugin.py`

 * *Files identical despite different names*

### Comparing `airflow-hop-plugin-0.1.0b3/airflow_hop/xml.py` & `airflow_hop_plugin-0.1.0b4/airflow_hop/xml.py`

 * *Files identical despite different names*

### Comparing `airflow-hop-plugin-0.1.0b3/airflow_hop_plugin.egg-info/PKG-INFO` & `airflow_hop_plugin-0.1.0b4/airflow_hop_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-hop-plugin
-Version: 0.1.0b3
+Version: 0.1.0b4
 Home-page: https://github.com/damavis/airflow-hop-plugin
 Author: Damavis
 Author-email: info@damavis.com
 License: Apache 2.0
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
```

### Comparing `airflow-hop-plugin-0.1.0b3/setup.py` & `airflow_hop_plugin-0.1.0b4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='airflow-hop-plugin',
-    version='0.1.0b3',
+    version='0.1.0b4',
     license='Apache 2.0',
     author='Damavis',
     author_email='info@damavis.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/damavis/airflow-hop-plugin',
     python_requires='>=3',
```

