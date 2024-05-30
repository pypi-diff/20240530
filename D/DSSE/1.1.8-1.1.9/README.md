# Comparing `tmp/dsse-1.1.8.tar.gz` & `tmp/dsse-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.1.8.tar", last modified: Thu May 23 21:03:27 2024, max compression
+gzip compressed data, was "dsse-1.1.9.tar", last modified: Thu May 30 15:49:43 2024, max compression
```

## Comparing `dsse-1.1.8.tar` & `dsse-1.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.537635 dsse-1.1.8/DSSE/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      322 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/__init__.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      490 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/constants.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7797 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/coverage_env.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/entities/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      686 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/drone.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8070 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/entities/person.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13388 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/env.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7509 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/env_base.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/imgs/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:19:41.000000 dsse-1.1.8/DSSE/environment/imgs/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/imgs/drone.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/environment/imgs/person-swimming.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4973 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/pygame_interface.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.541635 dsse-1.1.8/DSSE/environment/simulation/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4890 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/dynamic_probability.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7794 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/simulation/particle_simulation.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1205 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/environment/simulation/time_step.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE/environment/wrappers/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      417 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1505 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/all_flatten_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1701 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/all_positions_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1901 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/communication_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1391 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/gaussian_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1483 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/matrix_encode_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      975 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/retain_drone_pos_wrapper.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1963 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/environment/wrappers/top_n_cells_wrapper.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE/tests/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.8/DSSE/tests/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1488 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/tests/drone_policy.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    17985 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/tests/test_env.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6142 2024-05-23 20:55:10.000000 dsse-1.1.8/DSSE/tests/test_env_coverage.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      581 2024-04-18 19:38:11.000000 dsse-1.1.8/DSSE/tests/test_matrix.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-23 21:03:27.545635 dsse-1.1.8/DSSE.egg-info/
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8639 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1311 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      257 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/requires.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-05-23 21:03:27.000000 dsse-1.1.8/DSSE.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1094 2024-04-18 19:38:11.000000 dsse-1.1.8/LICENSE
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       32 2024-05-02 18:21:55.000000 dsse-1.1.8/MANIFEST.in
--rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8639 2024-05-23 21:03:27.545635 dsse-1.1.8/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6482 2024-05-23 20:55:10.000000 dsse-1.1.8/README.md
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2225 2024-05-23 20:55:10.000000 dsse-1.1.8/pyproject.toml
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-05-23 21:03:27.545635 dsse-1.1.8/setup.cfg
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      188 2024-05-23 21:02:01.000000 dsse-1.1.8/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.189099 dsse-1.1.9/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.181100 dsse-1.1.9/DSSE/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      322 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/__init__.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.181100 dsse-1.1.9/DSSE/environment/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.9/DSSE/environment/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      490 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/constants.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7797 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/coverage_env.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.181100 dsse-1.1.9/DSSE/environment/entities/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/entities/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      686 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/entities/drone.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8070 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/entities/person.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13388 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7509 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/env_base.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.181100 dsse-1.1.9/DSSE/environment/imgs/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:19:41.000000 dsse-1.1.9/DSSE/environment/imgs/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 dsse-1.1.9/DSSE/environment/imgs/drone.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 dsse-1.1.9/DSSE/environment/imgs/person-swimming.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4973 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/pygame_interface.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.185100 dsse-1.1.9/DSSE/environment/simulation/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/simulation/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4890 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/simulation/dynamic_probability.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7794 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/simulation/particle_simulation.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1205 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/environment/simulation/time_step.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.185100 dsse-1.1.9/DSSE/environment/wrappers/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      417 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1505 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/all_flatten_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1701 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/all_positions_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1901 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/communication_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1391 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/gaussian_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1483 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/matrix_encode_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      975 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/retain_drone_pos_wrapper.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1963 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/environment/wrappers/top_n_cells_wrapper.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.185100 dsse-1.1.9/DSSE/tests/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.9/DSSE/tests/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1488 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/tests/drone_policy.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    17985 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/tests/test_env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6142 2024-05-23 20:55:10.000000 dsse-1.1.9/DSSE/tests/test_env_coverage.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      581 2024-04-18 19:38:11.000000 dsse-1.1.9/DSSE/tests/test_matrix.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-30 15:49:43.185100 dsse-1.1.9/DSSE.egg-info/
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8785 2024-05-30 15:49:43.000000 dsse-1.1.9/DSSE.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1311 2024-05-30 15:49:43.000000 dsse-1.1.9/DSSE.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-05-30 15:49:43.000000 dsse-1.1.9/DSSE.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      257 2024-05-30 15:49:43.000000 dsse-1.1.9/DSSE.egg-info/requires.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-05-30 15:49:43.000000 dsse-1.1.9/DSSE.egg-info/top_level.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1094 2024-04-18 19:38:11.000000 dsse-1.1.9/LICENSE
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       32 2024-05-02 18:21:55.000000 dsse-1.1.9/MANIFEST.in
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     8785 2024-05-30 15:49:43.189099 dsse-1.1.9/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6628 2024-05-30 15:48:14.000000 dsse-1.1.9/README.md
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2225 2024-05-23 20:55:10.000000 dsse-1.1.9/pyproject.toml
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-05-30 15:49:43.189099 dsse-1.1.9/setup.cfg
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      188 2024-05-30 15:49:07.000000 dsse-1.1.9/setup.py
```

### Comparing `dsse-1.1.8/DSSE/environment/coverage_env.py` & `dsse-1.1.9/DSSE/environment/coverage_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/entities/drone.py` & `dsse-1.1.9/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/entities/person.py` & `dsse-1.1.9/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/env.py` & `dsse-1.1.9/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/env_base.py` & `dsse-1.1.9/DSSE/environment/env_base.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/imgs/drone.png` & `dsse-1.1.9/DSSE/environment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/imgs/person-swimming.png` & `dsse-1.1.9/DSSE/environment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/pygame_interface.py` & `dsse-1.1.9/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.9/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/simulation/particle_simulation.py` & `dsse-1.1.9/DSSE/environment/simulation/particle_simulation.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/simulation/time_step.py` & `dsse-1.1.9/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/all_flatten_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/all_flatten_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/all_positions_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/all_positions_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/communication_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/communication_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/gaussian_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/gaussian_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/matrix_encode_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/matrix_encode_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/retain_drone_pos_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/retain_drone_pos_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/environment/wrappers/top_n_cells_wrapper.py` & `dsse-1.1.9/DSSE/environment/wrappers/top_n_cells_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/tests/drone_policy.py` & `dsse-1.1.9/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/tests/test_env.py` & `dsse-1.1.9/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/tests/test_env_coverage.py` & `dsse-1.1.9/DSSE/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE/tests/test_matrix.py` & `dsse-1.1.9/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/DSSE.egg-info/PKG-INFO` & `dsse-1.1.9/DSSE.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.8
+Version: 1.1.9
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.8.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.9.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
@@ -41,15 +41,15 @@
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+# <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
 
 Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project offers a comprehensive simulation platform designed for developing, testing, and refining search strategies using drone swarms. Researchers and developers will find a versatile toolset supporting a broad spectrum of simulations, which facilitates the exploration of complex drone behaviors and interactions in dynamic, real-world scenarios.
 
 In this repository, we have implemented two distinct types of environments. The first is a dynamic environment that simulates maritime search and rescue operations for shipwreck survivors. It models the movement of individuals in the sea using a dynamic probability matrix, with the objective for drones being to locate and identify these individuals. The second is a environment utilizing the Lagrangian particle simulation from the open-source [Opendrift library](https://github.com/OpenDrift/opendrift), which incorporates real-world ocean and wind data to create a probability matrix for drone SAR tasks. In this scenario, drones are tasked with covering the full search area within the lowest time possible, while prioritizing higher probability areas.
 
 
 ## 📚 Documentation Links
@@ -60,15 +60,15 @@
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
 # DSSE - Search Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## 🎯 Outcome
 
 | If target is found       | If target is not found   |
@@ -129,15 +129,15 @@
 ```
 
 
 # DSSE - Coverage Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## ⚡ Quick Start
 
 ### ⚙️ Installation
```

### Comparing `dsse-1.1.8/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.9/DSSE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/LICENSE` & `dsse-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.1.8/PKG-INFO` & `dsse-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.8
+Version: 1.1.9
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.8.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/1.1.9.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
@@ -41,15 +41,15 @@
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+# <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
 
 Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project offers a comprehensive simulation platform designed for developing, testing, and refining search strategies using drone swarms. Researchers and developers will find a versatile toolset supporting a broad spectrum of simulations, which facilitates the exploration of complex drone behaviors and interactions in dynamic, real-world scenarios.
 
 In this repository, we have implemented two distinct types of environments. The first is a dynamic environment that simulates maritime search and rescue operations for shipwreck survivors. It models the movement of individuals in the sea using a dynamic probability matrix, with the objective for drones being to locate and identify these individuals. The second is a environment utilizing the Lagrangian particle simulation from the open-source [Opendrift library](https://github.com/OpenDrift/opendrift), which incorporates real-world ocean and wind data to create a probability matrix for drone SAR tasks. In this scenario, drones are tasked with covering the full search area within the lowest time possible, while prioritizing higher probability areas.
 
 
 ## 📚 Documentation Links
@@ -60,15 +60,15 @@
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
 # DSSE - Search Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## 🎯 Outcome
 
 | If target is found       | If target is not found   |
@@ -129,15 +129,15 @@
 ```
 
 
 # DSSE - Coverage Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## ⚡ Quick Start
 
 ### ⚙️ Installation
```

### Comparing `dsse-1.1.8/README.md` & `dsse-1.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+# <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
 
 Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project offers a comprehensive simulation platform designed for developing, testing, and refining search strategies using drone swarms. Researchers and developers will find a versatile toolset supporting a broad spectrum of simulations, which facilitates the exploration of complex drone behaviors and interactions in dynamic, real-world scenarios.
 
 In this repository, we have implemented two distinct types of environments. The first is a dynamic environment that simulates maritime search and rescue operations for shipwreck survivors. It models the movement of individuals in the sea using a dynamic probability matrix, with the objective for drones being to locate and identify these individuals. The second is a environment utilizing the Lagrangian particle simulation from the open-source [Opendrift library](https://github.com/OpenDrift/opendrift), which incorporates real-world ocean and wind data to create a probability matrix for drone SAR tasks. In this scenario, drones are tasked with covering the full search area within the lowest time possible, while prioritizing higher probability areas.
 
 
 ## 📚 Documentation Links
@@ -20,15 +20,15 @@
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
 # DSSE - Search Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## 🎯 Outcome
 
 | If target is found       | If target is not found   |
@@ -89,15 +89,15 @@
 ```
 
 
 # DSSE - Coverage Environment
 
 ## 🎥 Visual Demonstrations
 <p align="center">
-    <img src="docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
+    <img src="https://raw.githubusercontent.com/pfeinsper/drone-swarm-search/main/docs/public/gifs/basic_coverage.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
 ## ⚡ Quick Start
 
 ### ⚙️ Installation
```

### Comparing `dsse-1.1.8/pyproject.toml` & `dsse-1.1.9/pyproject.toml`

 * *Files identical despite different names*

