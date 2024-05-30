# Comparing `tmp/fenics_beat-0.0.6.tar.gz` & `tmp/fenics_beat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics_beat-0.0.6.tar", last modified: Mon May 27 14:37:16 2024, max compression
+gzip compressed data, was "fenics_beat-0.0.7.tar", last modified: Thu May 30 11:21:46 2024, max compression
```

## Comparing `fenics_beat-0.0.6.tar` & `fenics_beat-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.438603 fenics_beat-0.0.6/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/licenses/LICENSE_dolfin_pyvista_adapter
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:37:16.454603 fenics_beat-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.438603 fenics_beat-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.442603 fenics_beat-0.0.6/src/beat/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/bidomain_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.442603 fenics_beat-0.0.6/src/beat/cellmodels/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/beeler_reuter_1977.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/fitzhughnagumo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.446603 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.446603 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/endo.py
--rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/epi.py
--rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/mid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/conductivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/monodomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/single_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/src/beat/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.450603 fenics_beat-0.0.6/src/fenics_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 14:37:16.000000 fenics_beat-0.0.6/src/fenics_beat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:16.450603 fenics_beat-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_bidomain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_cellmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_monodomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_monodomain_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_odesolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_single_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 14:37:12.000000 fenics_beat-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.594466 fenics_beat-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 11:21:46.594466 fenics_beat-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.582466 fenics_beat-0.0.7/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/licenses/LICENSE_dolfin_pyvista_adapter
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:21:46.594466 fenics_beat-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.582466 fenics_beat-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.586466 fenics_beat-0.0.7/src/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/bidomain_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.586466 fenics_beat-0.0.7/src/beat/cellmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22492 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/beeler_reuter_1977.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/fitzhughnagumo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.586466 fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68630 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68719 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68702 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.586466 fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286750 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/endo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286758 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/epi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286743 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/mid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/conductivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/monodomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/src/beat/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.590466 fenics_beat-0.0.7/src/fenics_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-30 11:21:46.000000 fenics_beat-0.0.7/src/fenics_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-30 11:21:46.000000 fenics_beat-0.0.7/src/fenics_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:21:46.000000 fenics_beat-0.0.7/src/fenics_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-30 11:21:46.000000 fenics_beat-0.0.7/src/fenics_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 11:21:46.000000 fenics_beat-0.0.7/src/fenics_beat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:21:46.590466 fenics_beat-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_bidomain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_cellmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_monodomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_monodomain_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-30 11:21:41.000000 fenics_beat-0.0.7/tests/test_odesolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-30 11:21:42.000000 fenics_beat-0.0.7/tests/test_single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-30 11:21:42.000000 fenics_beat-0.0.7/tests/test_utils.py
```

### Comparing `fenics_beat-0.0.6/LICENSE` & `fenics_beat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/PKG-INFO` & `fenics_beat-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
```

### Comparing `fenics_beat-0.0.6/licenses/LICENSE_dolfin_pyvista_adapter` & `fenics_beat-0.0.7/licenses/LICENSE_dolfin_pyvista_adapter`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/pyproject.toml` & `fenics_beat-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-beat"
-version = "0.0.6"
+version = "0.0.7"
 description = "Library to run cardiac EP simulations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["cardiac", "electrophysiology"]
 dependencies = [
```

### Comparing `fenics_beat-0.0.6/src/beat/__init__.py` & `fenics_beat-0.0.7/src/beat/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/base_model.py` & `fenics_beat-0.0.7/src/beat/base_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/bidomain_model.py` & `fenics_beat-0.0.7/src/beat/bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/__init__.py` & `fenics_beat-0.0.7/src/beat/cellmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/beeler_reuter_1977.py` & `fenics_beat-0.0.7/src/beat/cellmodels/beeler_reuter_1977.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/fitzhughnagumo.py` & `fenics_beat-0.0.7/src/beat/cellmodels/fitzhughnagumo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py` & `fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py` & `fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py` & `fenics_beat-0.0.7/src/beat/cellmodels/tentusscher_panfilov_2006/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/endo.py` & `fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/endo.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/epi.py` & `fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/epi.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/cellmodels/torord_dyn_chloride/mid.py` & `fenics_beat-0.0.7/src/beat/cellmodels/torord_dyn_chloride/mid.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/conductivities.py` & `fenics_beat-0.0.7/src/beat/conductivities.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/ecg.py` & `fenics_beat-0.0.7/src/beat/ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/monodomain_model.py` & `fenics_beat-0.0.7/src/beat/monodomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/monodomain_solver.py` & `fenics_beat-0.0.7/src/beat/monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/odesolver.py` & `fenics_beat-0.0.7/src/beat/odesolver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/single_cell.py` & `fenics_beat-0.0.7/src/beat/single_cell.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/stimulation.py` & `fenics_beat-0.0.7/src/beat/stimulation.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/utils.py` & `fenics_beat-0.0.7/src/beat/utils.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/beat/viz.py` & `fenics_beat-0.0.7/src/beat/viz.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/src/fenics_beat.egg-info/PKG-INFO` & `fenics_beat-0.0.7/src/fenics_beat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-beat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library to run cardiac EP simulations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://finsberg.github.io/fenics-beat
 Project-URL: Documentation, https://finsberg.github.io/fenics-beat
 Project-URL: Source, https://github.com/finsberg/fenics-beat
 Project-URL: Tracker, https://github.com/finsberg/fenics-beat/issues
```

### Comparing `fenics_beat-0.0.6/src/fenics_beat.egg-info/SOURCES.txt` & `fenics_beat-0.0.7/src/fenics_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_bidomain_model.py` & `fenics_beat-0.0.7/tests/test_bidomain_model.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_cellmodels.py` & `fenics_beat-0.0.7/tests/test_cellmodels.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_ecg.py` & `fenics_beat-0.0.7/tests/test_ecg.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_monodomain.py` & `fenics_beat-0.0.7/tests/test_monodomain.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_monodomain_solver.py` & `fenics_beat-0.0.7/tests/test_monodomain_solver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_odesolver.py` & `fenics_beat-0.0.7/tests/test_odesolver.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_single_cell.py` & `fenics_beat-0.0.7/tests/test_single_cell.py`

 * *Files identical despite different names*

### Comparing `fenics_beat-0.0.6/tests/test_utils.py` & `fenics_beat-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

