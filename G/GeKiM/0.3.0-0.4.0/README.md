# Comparing `tmp/gekim-0.3.0.tar.gz` & `tmp/gekim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gekim-0.3.0.tar", last modified: Fri May 24 00:48:28 2024, max compression
+gzip compressed data, was "gekim-0.4.0.tar", last modified: Thu May 30 20:50:53 2024, max compression
```

## Comparing `gekim-0.3.0.tar` & `gekim-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/GeKiM.egg-info/
--rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1258 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/SOURCES.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/dependency_links.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/requires.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/top_level.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 gekim-0.3.0/LICENSE
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       24 2024-05-22 22:55:03.000000 gekim-0.3.0/MANIFEST.in
--rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-24 00:48:28.064759 gekim-0.3.0/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     2314 2024-05-23 22:14:30.000000 gekim-0.3.0/README.md
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      127 2024-05-23 23:54:52.000000 gekim-0.3.0/gekim/__init__.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       92 2024-05-23 21:48:57.000000 gekim-0.3.0/gekim/fields/__init__.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       87 2024-05-23 21:54:53.000000 gekim-0.3.0/gekim/fields/bio/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1028 2024-05-23 21:34:40.000000 gekim-0.3.0/gekim/fields/bio/binding.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:25.000000 gekim-0.3.0/gekim/fields/bio/cellular.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/enzyme/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       90 2024-05-23 21:52:20.000000 gekim-0.3.0/gekim/fields/bio/enzyme/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      582 2024-05-23 21:24:57.000000 gekim-0.3.0/gekim/fields/bio/enzyme/catalysis.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       67 2024-05-23 21:53:06.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    18191 2024-05-23 21:35:20.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/irrev.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:23:49.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/rev.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:32.000000 gekim-0.3.0/gekim/fields/bio/folding.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:14.000000 gekim-0.3.0/gekim/fields/bio/pharmaco.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:22.000000 gekim-0.3.0/gekim/fields/bio/population.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/chem/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-24 00:08:58.000000 gekim-0.3.0/gekim/fields/chem/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:36:10.000000 gekim-0.3.0/gekim/fields/chem/atmospheric.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      112 2024-05-23 21:33:23.000000 gekim-0.3.0/gekim/fields/chem/chem.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:28.000000 gekim-0.3.0/gekim/fields/chem/electro.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:39.000000 gekim-0.3.0/gekim/fields/chem/flow.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:20.000000 gekim-0.3.0/gekim/fields/chem/surface.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/fields/phys/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       57 2024-05-23 21:49:53.000000 gekim-0.3.0/gekim/fields/phys/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:57.000000 gekim-0.3.0/gekim/fields/phys/photo.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:41:04.000000 gekim-0.3.0/gekim/fields/phys/plasma.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:38:45.000000 gekim-0.3.0/gekim/fields/phys/quantum.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      151 2024-05-23 21:39:48.000000 gekim-0.3.0/gekim/fields/phys/stat_mech.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/schemes/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      134 2024-05-22 22:16:32.000000 gekim-0.3.0/gekim/schemes/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    20744 2024-05-22 22:22:06.000000 gekim-0.3.0/gekim/schemes/n_state.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/simulators/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      191 2024-05-14 23:49:52.000000 gekim-0.3.0/gekim/simulators/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1867 2024-05-15 23:52:27.000000 gekim-0.3.0/gekim/simulators/base_simulator.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     5290 2024-05-22 23:14:13.000000 gekim-0.3.0/gekim/simulators/gillespie.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    19942 2024-05-17 19:41:44.000000 gekim-0.3.0/gekim/simulators/ode_solver.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/utils/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      129 2024-05-23 16:25:14.000000 gekim-0.3.0/gekim/utils/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     7479 2024-05-17 22:41:27.000000 gekim-0.3.0/gekim/utils/fitting.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     4177 2024-05-16 22:45:21.000000 gekim-0.3.0/gekim/utils/helpers.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1877 2024-05-17 22:44:28.000000 gekim-0.3.0/gekim/utils/logging.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     3553 2024-05-14 18:10:03.000000 gekim-0.3.0/gekim/utils/plotting.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       93 2024-05-22 21:49:09.000000 gekim-0.3.0/pyproject.toml
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 21:21:28.000000 gekim-0.3.0/requirements.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-05-24 00:48:28.064759 gekim-0.3.0/setup.cfg
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      904 2024-05-24 00:47:42.000000 gekim-0.3.0/setup.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/tests/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    13184 2024-05-22 20:43:57.000000 gekim-0.3.0/tests/test_nstate_ode.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.646231 gekim-0.4.0/
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.646231 gekim-0.4.0/GeKiM.egg-info/
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-30 20:50:53.000000 gekim-0.4.0/GeKiM.egg-info/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1258 2024-05-30 20:50:53.000000 gekim-0.4.0/GeKiM.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-05-30 20:50:53.000000 gekim-0.4.0/GeKiM.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-30 20:50:53.000000 gekim-0.4.0/GeKiM.egg-info/requires.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-05-30 20:50:53.000000 gekim-0.4.0/GeKiM.egg-info/top_level.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 gekim-0.4.0/LICENSE
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       24 2024-05-22 22:55:03.000000 gekim-0.4.0/MANIFEST.in
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-30 20:50:53.646231 gekim-0.4.0/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     2314 2024-05-23 22:14:30.000000 gekim-0.4.0/README.md
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.638231 gekim-0.4.0/gekim/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      127 2024-05-23 23:54:52.000000 gekim-0.4.0/gekim/__init__.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.638231 gekim-0.4.0/gekim/fields/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       92 2024-05-23 21:48:57.000000 gekim-0.4.0/gekim/fields/__init__.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/fields/bio/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       87 2024-05-23 21:54:53.000000 gekim-0.4.0/gekim/fields/bio/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1028 2024-05-23 21:34:40.000000 gekim-0.4.0/gekim/fields/bio/binding.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:25.000000 gekim-0.4.0/gekim/fields/bio/cellular.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/fields/bio/enzyme/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       90 2024-05-23 21:52:20.000000 gekim-0.4.0/gekim/fields/bio/enzyme/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      582 2024-05-23 21:24:57.000000 gekim-0.4.0/gekim/fields/bio/enzyme/catalysis.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/fields/bio/enzyme/inhib/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       67 2024-05-23 21:53:06.000000 gekim-0.4.0/gekim/fields/bio/enzyme/inhib/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    18191 2024-05-23 21:35:20.000000 gekim-0.4.0/gekim/fields/bio/enzyme/inhib/irrev.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:23:49.000000 gekim-0.4.0/gekim/fields/bio/enzyme/inhib/rev.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:32.000000 gekim-0.4.0/gekim/fields/bio/folding.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:14.000000 gekim-0.4.0/gekim/fields/bio/pharmaco.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:22.000000 gekim-0.4.0/gekim/fields/bio/population.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/fields/chem/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-24 00:08:58.000000 gekim-0.4.0/gekim/fields/chem/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:36:10.000000 gekim-0.4.0/gekim/fields/chem/atmospheric.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      112 2024-05-23 21:33:23.000000 gekim-0.4.0/gekim/fields/chem/chem.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:28.000000 gekim-0.4.0/gekim/fields/chem/electro.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:39.000000 gekim-0.4.0/gekim/fields/chem/flow.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:20.000000 gekim-0.4.0/gekim/fields/chem/surface.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/fields/phys/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       57 2024-05-23 21:49:53.000000 gekim-0.4.0/gekim/fields/phys/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:57.000000 gekim-0.4.0/gekim/fields/phys/photo.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:41:04.000000 gekim-0.4.0/gekim/fields/phys/plasma.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:38:45.000000 gekim-0.4.0/gekim/fields/phys/quantum.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      151 2024-05-23 21:39:48.000000 gekim-0.4.0/gekim/fields/phys/stat_mech.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/schemes/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      134 2024-05-22 22:16:32.000000 gekim-0.4.0/gekim/schemes/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    20789 2024-05-30 20:37:35.000000 gekim-0.4.0/gekim/schemes/n_state.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/simulators/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      191 2024-05-14 23:49:52.000000 gekim-0.4.0/gekim/simulators/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1867 2024-05-15 23:52:27.000000 gekim-0.4.0/gekim/simulators/base_simulator.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     5290 2024-05-22 23:14:13.000000 gekim-0.4.0/gekim/simulators/gillespie.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    19738 2024-05-30 20:49:05.000000 gekim-0.4.0/gekim/simulators/ode_solver.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.642231 gekim-0.4.0/gekim/utils/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      129 2024-05-23 16:25:14.000000 gekim-0.4.0/gekim/utils/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     8185 2024-05-28 20:22:38.000000 gekim-0.4.0/gekim/utils/fitting.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     4948 2024-05-28 21:46:49.000000 gekim-0.4.0/gekim/utils/helpers.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1877 2024-05-17 22:44:28.000000 gekim-0.4.0/gekim/utils/logging.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     3553 2024-05-14 18:10:03.000000 gekim-0.4.0/gekim/utils/plotting.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       93 2024-05-22 21:49:09.000000 gekim-0.4.0/pyproject.toml
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 21:21:28.000000 gekim-0.4.0/requirements.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-05-30 20:50:53.646231 gekim-0.4.0/setup.cfg
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      904 2024-05-30 20:50:24.000000 gekim-0.4.0/setup.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-30 20:50:53.646231 gekim-0.4.0/tests/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    13191 2024-05-30 20:45:56.000000 gekim-0.4.0/tests/test_nstate_ode.py
```

### Comparing `gekim-0.3.0/GeKiM.egg-info/PKG-INFO` & `gekim-0.4.0/GeKiM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeKiM
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.
 Home-page: https://github.com/kghaby/GeKiM
 Author: Kyle Ghaby
 Author-email: kyleghaby@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
```

### Comparing `gekim-0.3.0/GeKiM.egg-info/SOURCES.txt` & `gekim-0.4.0/GeKiM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/LICENSE` & `gekim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/PKG-INFO` & `gekim-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeKiM
-Version: 0.3.0
+Version: 0.4.0
 Summary: Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.
 Home-page: https://github.com/kghaby/GeKiM
 Author: Kyle Ghaby
 Author-email: kyleghaby@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
```

### Comparing `gekim-0.3.0/README.md` & `gekim-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/fields/bio/binding.py` & `gekim-0.4.0/gekim/fields/bio/binding.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/fields/bio/enzyme/catalysis.py` & `gekim-0.4.0/gekim/fields/bio/enzyme/catalysis.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/fields/bio/enzyme/inhib/irrev.py` & `gekim-0.4.0/gekim/fields/bio/enzyme/inhib/irrev.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/schemes/n_state.py` & `gekim-0.4.0/gekim/schemes/n_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
 import re
 import copy
 from sympy import symbols
 from collections import defaultdict
+from typing import Union
 from ..utils.helpers import integerable_float
 from ..utils.logging import Logger
     
 class Species:
-    def __init__(self, name: str, y0: np.ndarray | float, label=None, color=None):
+    def __init__(self, name: str, y0: Union[np.ndarray,float], label=None, color=None):
             """
             Initialize a species object.
 
             Parameters
             ----------
             name : str
                 Name of the species.
-            y0 : np.ndarray | float
+            y0 : Union[np.ndarray,float]
                 Initial concentration of the species.
                 Array Example: `{"Ligand":np.linspace(1,1500,100)}` for a Michaelis-Menten ligand concentration scan.
             label : str, optional
                 Useful for plotting. Will default to NAME.
             color : str, optional
                 Useful for plotting. Best added by ..utils.Plotting.assign_colors_to_species().
 
@@ -373,15 +374,15 @@
         Useful for saving the output of a continuous solution to the species dictionary.
         Don't forget to save time, too, eg `system.simout["t_cont"] = t`
         """
         for _, sp_data in self.species.items():
             sp_data.simout[key_name] = matrix[sp_data.index]
         return
 
-    def find_paths(self, start_species: str | Species, end_species: str | Species, only_linear_paths=True, 
+    def find_paths(self, start_species: Union[str,Species], end_species: Union[str,Species], only_linear_paths=True, 
                    prob_cutoff=1e-10, max_depth=20, log_paths=False, normalize_prob=True):
         """
         Find paths from start_species to end_species.
 
         Parameters
         ----------
         start_species : str or Species
```

### Comparing `gekim-0.3.0/gekim/simulators/base_simulator.py` & `gekim-0.4.0/gekim/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/simulators/gillespie.py` & `gekim-0.4.0/gekim/simulators/gillespie.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/simulators/ode_solver.py` & `gekim-0.4.0/gekim/simulators/ode_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,21 @@
         """
         (Re)initialize the simulator by generating the necessary matrices and symbolic expressions, 
         and saving them to the system and species simin dictionaries.
         """
         
         self._generate_matrices_for_rates_func() 
 
-        sp_syms = {name: symbols(name) for name in self.system.species}
-        tr_syms = {name: symbols(name) for name in self.system.transitions}
-
         # Rate laws 
-        self._generate_rates_sym(sp_syms,tr_syms) 
+        self._generate_rates_sym() 
         self.log_rates()
-        #self._lambdify_sym_rates(sp_syms) # Overwrites self._rates_func with a lambdified version of self.system.simin["rates_sym"]
+        #self.lambdify_sym_rates() # Overwrites self._rates_func with a lambdified version of self.system.simin["rates_sym"]
 
         # Jacobian
-        self._generate_jac(sp_syms) # generates self.system.simin["J_sym"], self.system.simin["J_symsp_numtr"], self.system.simin["J_func_wrap"]
+        self._generate_jac() # generates self.system.simin["J_sym"], self.system.simin["J_symsp_numtr"], self.system.simin["J_func_wrap"]
         self.log_jac()
 
     def _generate_matrices_for_rates_func(self):
         """
         Notes
         -----
         Generates 
@@ -113,28 +110,28 @@
         """
         #TODO: Use higher dimensionality conc arrays to process multiple input concs at once? 
         C_Nr = np.prod(np.power(conc, self.system.simin["stoich_reactant_mat"]), axis=1) # state dependencies
         N_K = np.dot(self.system.simin["k_diag"],self.system.simin["stoich_mat"]) # interactions
         rates = np.dot(C_Nr,N_K)
         return rates
     
-    def _generate_rates_sym(self,sp_syms,tr_syms):
+    def _generate_rates_sym(self):
         """
         Notes
         -----
         Generates 
         - Species rate vectors with symbolic species and rate constants 
         - Species rate vectors with symbolic species and numerical rate constants
 
         Adds these key/value pairs to both system and species simin dictionaries.
         """
         # Generate rate's with symbolic species and rate constants 
-        rates_sym = Matrix([0] * len(sp_syms))
+        rates_sym = Matrix([0] * len(self.system.species))
         for tr_name, tr in self.system.transitions.items():
-            unscaled_rate = tr_syms[tr_name] * prod(sp_syms[sp_name]**coeff for sp_name, coeff in tr.source)
+            unscaled_rate = self.system.transitions[tr_name].sym * prod(self.system.species[sp_name].sym**coeff for sp_name, coeff in tr.source)
             for sp_name, coeff in tr.source:
                 rates_sym[self.system.species[sp_name].index] -= coeff * unscaled_rate
             for sp_name, coeff in tr.target:
                 rates_sym[self.system.species[sp_name].index] += coeff * unscaled_rate
         self.system.simin["rates_sym"] = rates_sym 
         self.system.log.info("Saved rates_sym and rates_numk into system simin dict (SYSTEM.simin).")
 
@@ -146,24 +143,23 @@
         for sp_name, sp_data in self.system.species.items():
             sp_data.simin["rate_sym"] = self.system.simin["rates_sym"][sp_data.index]
             sp_data.simin["rate_numk"] = self.system.simin["rates_numk"][sp_data.index]
         self.system.log.info("Saved rate_sym and rate_numk into species simin dict (SYSTEM.species[NAME].simin).")
 
         return 
     
-    def _lambdify_sym_rates(self,sp_syms):
+    def lambdify_sym_rates(self):
         """
         Convert the symbolic rate vector (with numerical rate constants) into a numerical function.
 
         Notes
         -----
-        This overwrites the native self._rate function. It's just as fast typically, if not a little faster.
-        Not currently utilized, but this might be useful someday.
+        This overwrites the unsymbolic self._rates_func function.
         """
-        species_vec = Matrix([sp_syms[name] for name in self.system.species])
+        species_vec = Matrix([self.system.species[sp_name].sym for sp_name in self.system.species])
         rates_func = lambdify(species_vec, self.system.simin["rates_numk"], 'numpy')
         self._rates_func = lambda t, y: rates_func(*y).flatten()
         return
 
     def log_rates(self,force_print=False):
         """
         Log the symbolic rates using the system's logger.
@@ -211,30 +207,30 @@
             rate_log += formatted_eqn + '\n\n'
 
         self.system.log.info(rate_log)
         if force_print:
             print(rate_log)
         return
 
-    def _generate_jac(self,sp_syms):
+    def _generate_jac(self):
         """
         Notes
         -----
         Generates
          - the Jacobian matrix with symbolic species and rate constants (self.system.simin["J_sym"])
          - the Jacobian matrix with symbolic species and numerical rate constants (self.system.simin["J_symsp_numtr"])
          - a wrapped numerical Jacobian function (self.system.simin["J_func_wrap"]) that accepts t,y as arguments
 
         The wrapped numerical function is time-independent even though it accepts t as an argument!
 
         The Jacobian matrix here represents the first-order partial derivatives of the rate of 
             change equations for each species with respect to all other species in the system.
         """
         
-        species_vec = Matrix(list(sp_syms.values()))
+        species_vec = Matrix([self.system.species[sp_name].sym for sp_name in self.system.species])
 
         # Symbolic Jacobian
         self.system.simin["J_sym"] = self.system.simin["rates_sym"].jacobian(species_vec)
 
         # Numerical Jacobian
         self.system.simin["J_symsp_numtr"] = self.system.simin["rates_numk"].jacobian(species_vec) # Symbolic species, numeric transition rate constants
         J_func = lambdify(species_vec, self.system.simin["J_symsp_numtr"], 'numpy') # Make numerical function
```

### Comparing `gekim-0.3.0/gekim/utils/fitting.py` & `gekim-0.4.0/gekim/utils/fitting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np
 import inspect
 from sympy import symbols, Matrix, lambdify
+from scipy.optimize import curve_fit
+from scipy.stats import gaussian_kde
+from .helpers import update_dict_with_subset
+
 #TODO: scheme fitting, rate constant fitting
 
 def chi_squared(observed_data: np.ndarray, fitted_data: np.ndarray, fitted_params: np.ndarray, variances: np.ndarray = None, reduced=False):
     """
     Calculate the chi-squared and optionally the reduced chi-squared statistics.
 
     Parameters
@@ -200,8 +204,30 @@
     ss_res = np.sum(residuals**2)
     ss_tot = np.sum((y_obs - np.mean(y_obs))**2)
     r_squared = 1 - (ss_res / ss_tot)
     if r_squared < 0.5:
         bad = True
         message += f"\n\tLow R² value: {r_squared:.2e}"
 
-    return bad, message
+    return bad, message
+
+def calc_nrmse(y_exp: np.ndarray, y_pred: np.ndarray):
+    """
+    Calculate the Normalized Root Mean Squared Error (NRMSE) between two arrays.
+
+    Parameters
+    ----------
+    y_exp : np.ndarray
+        Array of experimental values.
+    y_pred : np.ndarray
+        Array of predicted values.
+
+    Returns
+    -------
+    float
+        NRMSE value between 0 and 1, where 1 is a perfect match.
+    """
+    mse = np.mean((y_exp - y_pred) ** 2)
+    rmse = np.sqrt(mse)
+    range_y = np.ptp(y_exp)  # Equivalent to max(y_exp) - min(y_exp)
+    nrmse = 1 - rmse / range_y
+    return nrmse
```

### Comparing `gekim-0.3.0/gekim/utils/helpers.py` & `gekim-0.4.0/gekim/utils/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import math
-
+from itertools import product
 
 
 def rate_pair_from_P(int_OOM,P_B) -> tuple:
     """
     Provides rates between two states that are at rapid equilibrium and 
         therefore approximated by the population distribution. 
 
@@ -31,15 +31,15 @@
     Returns a float as an integer if it is an integer, otherwise returns the float.
     """
     if num.is_integer():
         return int(num)
     else:
         return num
     
-def round_sig(num, sig_figs, autoformat=True):
+def round_sig(num: float, sig_figs: int = 3, autoformat=True):
     """
     Round up using significant figures.
 
     Parameters:
     ----------
     num : float
         The number to be rounded.
@@ -133,7 +133,32 @@
         else:
             arr1, arr2 = np.array(value1), np.array(value2)
             if not np.allclose(arr1, arr2, rtol=rel_tol, atol=abs_tol):
                 return False
     return True
 
 
+
+def generate_dictval_combinations(input_dict: dict):
+    """
+    Generate all combinations of values in a dictionary and return them as a dictionary
+    with the original keys and numpy arrays of corresponding values.
+
+    Parameters
+    ----------
+    input_dict : dict
+        Keys are parameter names and values are numpy arrays.
+
+    Returns
+    -------
+    dict
+        Dictionary with the original keys and numpy arrays of corresponding value
+    """
+
+    names = list(input_dict.keys())
+    values = list(input_dict.values())
+
+    combinations = list(product(*values))
+    combinations_array = np.array(combinations).T
+
+    comb_dict = {name: combinations_array[i] for i, name in enumerate(names)}
+    return comb_dict
```

### Comparing `gekim-0.3.0/gekim/utils/logging.py` & `gekim-0.4.0/gekim/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/gekim/utils/plotting.py` & `gekim-0.4.0/gekim/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gekim-0.3.0/setup.py` & `gekim-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='GeKiM', 
-    version='0.3.0', 
+    version='0.4.0', 
     author='Kyle Ghaby', 
     author_email='kyleghaby@gmail.com',  
     description='Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.',  
     long_description=open('README.md').read(),  
     long_description_content_type='text/markdown',
     url='https://github.com/kghaby/GeKiM', 
     packages=find_packages(),
```

### Comparing `gekim-0.3.0/tests/test_nstate_ode.py` & `gekim-0.4.0/tests/test_nstate_ode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import gekim as gk
-import gekim.analysis.covalent_inhibition as ci
+from gekim.fields.bio.enzyme.inhib import irrev as ii 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.integrate import solve_ivp
 
 # Test whether gekim NState systems yield the same output as hardcoded systems
 
 # User option to plot time course of NState systems (will still plot on mismatch)
@@ -130,15 +130,15 @@
 for name,scheme in schemes.items():
     system = gk.schemes.NState(scheme,quiet=True)
     #sol = _solve_odes_old(system,t,output_raw=True) #testing with old (nonvectorized) version
     system.set_simulator(gk.simulators.ODESolver)
     sol = system.simulator.simulate(t_eval=t,output_raw=True,atol=1e-8,rtol=1e-6)
     final_state = system.species["EI"].simout["y"]
     all_bound = system.sum_species_simout(blacklist=["E","I"])
-    fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+    fit_output = ii.kobs_uplim_fit_to_occ_final_wrt_t(
         t,final_state,nondefault_params={"Etot":{"fix":concE0}})
     schemes[name]["fit_output"] = fit_output
     schemes[name]["sol"] = sol
     
     if PLOT:
         fig = plt.figure(figsize=(5, 3))
 
@@ -298,15 +298,15 @@
         plt.tight_layout()
         plt.show()
 
 # Solve hardcoded systems
 def solve_system(system,t,concE0):
     sol = system.solve(t)
     final_state = sol.y[-1]
-    fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+    fit_output = ii.kobs_uplim_fit_to_occ_final_wrt_t(
         t,final_state,nondefault_params={"Etot":{"fix":concE0}})
     system_dict = {
         "system": system,
         "sol": sol,
         "final_state": final_state,
         "fit_output": fit_output
     }
```

