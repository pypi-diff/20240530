# Comparing `tmp/biosimulator-processes-0.0.8.tar.gz` & `tmp/biosimulator-processes-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosimulator-processes-0.0.8.tar", last modified: Mon Jan  8 21:28:43 2024, max compression
+gzip compressed data, was "biosimulator-processes-0.0.9.tar", last modified: Mon Jan  8 21:31:13 2024, max compression
```

## Comparing `biosimulator-processes-0.0.8.tar` & `biosimulator-processes-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:28:43.442713 biosimulator-processes-0.0.8/
--rw-r--r--   0 alex       (501) staff       (20)      143 2023-11-25 01:06:53.000000 biosimulator-processes-0.0.8/AUTHORS.md
--rw-r--r--   0 alex       (501) staff       (20)    11358 2023-11-25 01:06:53.000000 biosimulator-processes-0.0.8/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     3171 2024-01-08 21:28:43.442497 biosimulator-processes-0.0.8/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1914 2024-01-08 21:21:14.000000 biosimulator-processes-0.0.8/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:28:43.440522 biosimulator-processes-0.0.8/biosimulator_processes/
--rw-r--r--   0 alex       (501) staff       (20)       22 2024-01-08 21:28:18.000000 biosimulator-processes-0.0.8/biosimulator_processes/_VERSION.py
--rw-r--r--   0 alex       (501) staff       (20)      676 2024-01-08 21:15:17.000000 biosimulator-processes-0.0.8/biosimulator_processes/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-12-18 16:55:33.000000 biosimulator-processes-0.0.8/biosimulator_processes/biosimulator_process.py
--rw-r--r--   0 alex       (501) staff       (20)     1884 2024-01-08 21:12:01.000000 biosimulator-processes-0.0.8/biosimulator_processes/cobra_process.py
--rw-r--r--   0 alex       (501) staff       (20)     4492 2024-01-08 20:43:21.000000 biosimulator-processes-0.0.8/biosimulator_processes/copasi_process.py
--rw-r--r--   0 alex       (501) staff       (20)    14274 2024-01-06 00:21:07.000000 biosimulator-processes-0.0.8/biosimulator_processes/smoldyn_process.py
--rw-r--r--   0 alex       (501) staff       (20)     6614 2024-01-06 00:47:46.000000 biosimulator-processes-0.0.8/biosimulator_processes/tellurium_process.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:28:43.441947 biosimulator-processes-0.0.8/biosimulator_processes/tests/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-12-14 17:54:31.000000 biosimulator-processes-0.0.8/biosimulator_processes/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1345 2024-01-05 17:35:29.000000 biosimulator-processes-0.0.8/biosimulator_processes/tests/test_cobra.py
--rw-r--r--   0 alex       (501) staff       (20)     1753 2024-01-08 20:52:19.000000 biosimulator-processes-0.0.8/biosimulator_processes/tests/test_copasi.py
--rw-r--r--   0 alex       (501) staff       (20)     2524 2024-01-08 21:27:52.000000 biosimulator-processes-0.0.8/biosimulator_processes/tests/test_smoldyn.py
--rw-r--r--   0 alex       (501) staff       (20)     5255 2024-01-08 21:27:43.000000 biosimulator-processes-0.0.8/biosimulator_processes/tests/test_tellurium.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:28:43.441130 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     3171 2024-01-08 21:28:43.000000 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      770 2024-01-08 21:28:43.000000 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-01-08 21:28:43.000000 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      113 2024-01-08 21:28:43.000000 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       23 2024-01-08 21:28:43.000000 biosimulator-processes-0.0.8/biosimulator_processes.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-01-08 21:28:43.442782 biosimulator-processes-0.0.8/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1887 2024-01-08 20:58:29.000000 biosimulator-processes-0.0.8/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:31:13.741318 biosimulator-processes-0.0.9/
+-rw-r--r--   0 alex       (501) staff       (20)      143 2023-11-25 01:06:53.000000 biosimulator-processes-0.0.9/AUTHORS.md
+-rw-r--r--   0 alex       (501) staff       (20)    11358 2023-11-25 01:06:53.000000 biosimulator-processes-0.0.9/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     3171 2024-01-08 21:31:13.741104 biosimulator-processes-0.0.9/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1914 2024-01-08 21:21:14.000000 biosimulator-processes-0.0.9/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:31:13.739008 biosimulator-processes-0.0.9/biosimulator_processes/
+-rw-r--r--   0 alex       (501) staff       (20)       22 2024-01-08 21:30:59.000000 biosimulator-processes-0.0.9/biosimulator_processes/_VERSION.py
+-rw-r--r--   0 alex       (501) staff       (20)      676 2024-01-08 21:15:17.000000 biosimulator-processes-0.0.9/biosimulator_processes/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-12-18 16:55:33.000000 biosimulator-processes-0.0.9/biosimulator_processes/biosimulator_process.py
+-rw-r--r--   0 alex       (501) staff       (20)     1884 2024-01-08 21:12:01.000000 biosimulator-processes-0.0.9/biosimulator_processes/cobra_process.py
+-rw-r--r--   0 alex       (501) staff       (20)     4492 2024-01-08 20:43:21.000000 biosimulator-processes-0.0.9/biosimulator_processes/copasi_process.py
+-rw-r--r--   0 alex       (501) staff       (20)    14274 2024-01-06 00:21:07.000000 biosimulator-processes-0.0.9/biosimulator_processes/smoldyn_process.py
+-rw-r--r--   0 alex       (501) staff       (20)     6614 2024-01-06 00:47:46.000000 biosimulator-processes-0.0.9/biosimulator_processes/tellurium_process.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:31:13.740633 biosimulator-processes-0.0.9/biosimulator_processes/tests/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-12-14 17:54:31.000000 biosimulator-processes-0.0.9/biosimulator_processes/tests/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1345 2024-01-05 17:35:29.000000 biosimulator-processes-0.0.9/biosimulator_processes/tests/test_cobra.py
+-rw-r--r--   0 alex       (501) staff       (20)     1753 2024-01-08 20:52:19.000000 biosimulator-processes-0.0.9/biosimulator_processes/tests/test_copasi.py
+-rw-r--r--   0 alex       (501) staff       (20)     2524 2024-01-08 21:27:52.000000 biosimulator-processes-0.0.9/biosimulator_processes/tests/test_smoldyn.py
+-rw-r--r--   0 alex       (501) staff       (20)     5255 2024-01-08 21:27:43.000000 biosimulator-processes-0.0.9/biosimulator_processes/tests/test_tellurium.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-01-08 21:31:13.739767 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3171 2024-01-08 21:31:13.000000 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      770 2024-01-08 21:31:13.000000 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-01-08 21:31:13.000000 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      113 2024-01-08 21:31:13.000000 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       23 2024-01-08 21:31:13.000000 biosimulator-processes-0.0.9/biosimulator_processes.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-01-08 21:31:13.741368 biosimulator-processes-0.0.9/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1887 2024-01-08 20:58:29.000000 biosimulator-processes-0.0.9/setup.py
```

### Comparing `biosimulator-processes-0.0.8/LICENSE` & `biosimulator-processes-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/PKG-INFO` & `biosimulator-processes-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulator-processes
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/vivarium-collective/process-bigraph
 Author: Ryan Spangler, Eran Agmon, Alex Patrie
 Author-email: ryan.spangler@gmail.com, agmon.eran@gmail.com, alexanderpatrie@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `biosimulator-processes-0.0.8/README.md` & `biosimulator-processes-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/__init__.py` & `biosimulator-processes-0.0.9/biosimulator_processes/__init__.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/cobra_process.py` & `biosimulator-processes-0.0.9/biosimulator_processes/cobra_process.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/copasi_process.py` & `biosimulator-processes-0.0.9/biosimulator_processes/copasi_process.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/smoldyn_process.py` & `biosimulator-processes-0.0.9/biosimulator_processes/smoldyn_process.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/tellurium_process.py` & `biosimulator-processes-0.0.9/biosimulator_processes/tellurium_process.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/tests/test_cobra.py` & `biosimulator-processes-0.0.9/biosimulator_processes/tests/test_cobra.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/tests/test_copasi.py` & `biosimulator-processes-0.0.9/biosimulator_processes/tests/test_copasi.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/tests/test_smoldyn.py` & `biosimulator-processes-0.0.9/biosimulator_processes/tests/test_smoldyn.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes/tests/test_tellurium.py` & `biosimulator-processes-0.0.9/biosimulator_processes/tests/test_tellurium.py`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes.egg-info/PKG-INFO` & `biosimulator-processes-0.0.9/biosimulator_processes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosimulator-processes
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/vivarium-collective/process-bigraph
 Author: Ryan Spangler, Eran Agmon, Alex Patrie
 Author-email: ryan.spangler@gmail.com, agmon.eran@gmail.com, alexanderpatrie@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `biosimulator-processes-0.0.8/biosimulator_processes.egg-info/SOURCES.txt` & `biosimulator-processes-0.0.9/biosimulator_processes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosimulator-processes-0.0.8/setup.py` & `biosimulator-processes-0.0.9/setup.py`

 * *Files identical despite different names*

