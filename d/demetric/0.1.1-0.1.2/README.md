# Comparing `tmp/demetric-0.1.1.tar.gz` & `tmp/demetric-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demetric-0.1.1.tar", last modified: Thu May 30 20:27:55 2024, max compression
+gzip compressed data, was "demetric-0.1.2.tar", last modified: Thu May 30 20:29:22 2024, max compression
```

## Comparing `demetric-0.1.1.tar` & `demetric-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:27:55.886665 demetric-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-30 20:27:55.886665 demetric-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      350 2024-05-30 20:27:49.000000 demetric-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      552 2024-05-30 20:27:53.000000 demetric-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 20:27:55.886665 demetric-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:27:55.876665 demetric-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:27:55.886665 demetric-0.1.1/src/demetric/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.1/src/demetric/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      160 2024-05-30 20:20:05.000000 demetric-0.1.1/src/demetric/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      329 2024-05-30 20:13:40.000000 demetric-0.1.1/src/demetric/comparing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2166 2024-05-30 20:23:30.000000 demetric-0.1.1/src/demetric/experiment.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:27:55.886665 demetric-0.1.1/src/demetric/plot/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-30 20:07:20.000000 demetric-0.1.1/src/demetric/plot/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       74 2024-05-30 20:08:49.000000 demetric-0.1.1/src/demetric/plot/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-05-30 20:13:48.000000 demetric-0.1.1/src/demetric/plot/_plot.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      445 2024-05-30 20:24:44.000000 demetric-0.1.1/src/demetric/runs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:27:55.886665 demetric-0.1.1/src/demetric.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-05-30 20:27:55.000000 demetric-0.1.1/src/demetric.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-05-30 20:27:55.000000 demetric-0.1.1/src/demetric.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 20:27:55.000000 demetric-0.1.1/src/demetric.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-05-30 20:27:55.000000 demetric-0.1.1/src/demetric.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-30 20:27:55.000000 demetric-0.1.1/src/demetric.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:29:22.486667 demetric-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      762 2024-05-30 20:29:22.486667 demetric-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      447 2024-05-30 20:29:07.000000 demetric-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      552 2024-05-30 20:29:20.000000 demetric-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-30 20:29:22.486667 demetric-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:29:22.476667 demetric-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:29:22.486667 demetric-0.1.2/src/demetric/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.2/src/demetric/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      160 2024-05-30 20:20:05.000000 demetric-0.1.2/src/demetric/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      329 2024-05-30 20:13:40.000000 demetric-0.1.2/src/demetric/comparing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2166 2024-05-30 20:23:30.000000 demetric-0.1.2/src/demetric/experiment.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:29:22.486667 demetric-0.1.2/src/demetric/plot/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-30 20:07:20.000000 demetric-0.1.2/src/demetric/plot/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       74 2024-05-30 20:08:49.000000 demetric-0.1.2/src/demetric/plot/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-05-30 20:13:48.000000 demetric-0.1.2/src/demetric/plot/_plot.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      445 2024-05-30 20:24:44.000000 demetric-0.1.2/src/demetric/runs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-30 20:29:22.486667 demetric-0.1.2/src/demetric.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      762 2024-05-30 20:29:22.000000 demetric-0.1.2/src/demetric.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      416 2024-05-30 20:29:22.000000 demetric-0.1.2/src/demetric.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-30 20:29:22.000000 demetric-0.1.2/src/demetric.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        7 2024-05-30 20:29:22.000000 demetric-0.1.2/src/demetric.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-30 20:29:22.000000 demetric-0.1.2/src/demetric.egg-info/top_level.txt
```

### Comparing `demetric-0.1.1/PKG-INFO` & `demetric-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demetric
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple and composable metric tracking and logging for ML
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 
@@ -23,7 +23,19 @@
 exp.log('loss', value=loss, step=step)
 exp.log('accuracy', value=acc, step=step)
 
 
 fig, ax = exp.plot('loss')
 fig2, ax2 = exp.plot_summary()
 ```
+
+
+Creates:
+
+```
+runs/
+  gpt2-3/
+    meta.json
+    metrics/
+      loss.csv
+      accuracy.csv
+```
```

### Comparing `demetric-0.1.1/pyproject.toml` & `demetric-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "demetric"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple and composable metric tracking and logging for ML"
 dependencies = [
   "pandas",
 ]
```

### Comparing `demetric-0.1.1/src/demetric/experiment.py` & `demetric-0.1.2/src/demetric/experiment.py`

 * *Files identical despite different names*

### Comparing `demetric-0.1.1/src/demetric.egg-info/PKG-INFO` & `demetric-0.1.2/src/demetric.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demetric
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple and composable metric tracking and logging for ML
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 
@@ -23,7 +23,19 @@
 exp.log('loss', value=loss, step=step)
 exp.log('accuracy', value=acc, step=step)
 
 
 fig, ax = exp.plot('loss')
 fig2, ax2 = exp.plot_summary()
 ```
+
+
+Creates:
+
+```
+runs/
+  gpt2-3/
+    meta.json
+    metrics/
+      loss.csv
+      accuracy.csv
+```
```

