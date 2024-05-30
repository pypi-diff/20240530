# Comparing `tmp/TSC2018_Design-1.1.4.tar.gz` & `tmp/tsc2018_design-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSC2018_Design-1.1.4.tar", last modified: Wed Mar 20 09:42:22 2024, max compression
+gzip compressed data, was "tsc2018_design-1.1.5.tar", last modified: Thu May 30 13:32:17 2024, max compression
```

## Comparing `TSC2018_Design-1.1.4.tar` & `tsc2018_design-1.1.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.039687 TSC2018_Design-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-03-20 09:42:22.039687 TSC2018_Design-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 09:42:22.039687 TSC2018_Design-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.031687 TSC2018_Design-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.031687 TSC2018_Design-1.1.4/src/TSC/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.031687 TSC2018_Design-1.1.4/src/TSC/Design/
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/ConfimentBarsRules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/Definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/Frp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/GlobalParamCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)    27088 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/MaterialModels.py
--rw-r--r--   0 runner    (1001) docker     (127)    31794 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/ResponseSpectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/SeismicLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Design/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.035687 TSC2018_Design-1.1.4/src/TSC/MSCSI/
--rw-r--r--   0 runner    (1001) docker     (127)   143912 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/AnalysisResult.py
--rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/CaseStaticNonlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Combo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Database.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/ErrorHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/FunctionRS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/LoadCases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/LoadPattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/MaterialProp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/PluginCallback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/Story.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/MSCSI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.035687 TSC2018_Design-1.1.4/src/TSC/Resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.035687 TSC2018_Design-1.1.4/src/TSC/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Utility/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/src/TSC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.039687 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-03-20 09:42:22.000000 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-20 09:42:22.000000 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 09:42:22.000000 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-20 09:42:22.000000 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 09:42:22.000000 TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 09:42:22.039687 TSC2018_Design-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/tests/test_FRP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-20 09:42:18.000000 TSC2018_Design-1.1.4/tests/test_TSCConfinmentBarsRules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.039914 tsc2018_design-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:32:17.039914 tsc2018_design-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.027914 tsc2018_design-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.027914 tsc2018_design-1.1.5/src/TSC/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.031914 tsc2018_design-1.1.5/src/TSC/Design/
+-rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/ConfimentBarsRules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/Definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/Frp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/GlobalParamCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27088 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/MaterialModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32253 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/ResponseSpectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/SeismicLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Design/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/src/TSC/MSCSI/
+-rw-r--r--   0 runner    (1001) docker     (127)   143988 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/AnalysisResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/CaseStaticNonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Combo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/ErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/FunctionRS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45614 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/LoadCases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/LoadPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/MaterialProp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/PluginCallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/Story.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/MSCSI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/src/TSC/Resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/src/TSC/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Utility/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/src/TSC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-30 13:32:17.000000 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-30 13:32:17.000000 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:32:17.000000 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 13:32:17.000000 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 13:32:17.000000 tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:32:17.035914 tsc2018_design-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/tests/test_FRP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/tests/test_MSCSI_LoadCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 13:32:13.000000 tsc2018_design-1.1.5/tests/test_TSCConfinmentBarsRules.py
```

### Comparing `TSC2018_Design-1.1.4/LICENSE` & `tsc2018_design-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/PKG-INFO` & `tsc2018_design-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSC2018_Design
-Version: 1.1.4
+Version: 1.1.5
 Summary: TSC2018 design
 Author-email: Muhammed Sural <muhammedsural@gmail.com>
 Project-URL: Homepage, https://github.com/muhammedsural/TSC2018_Design
 Project-URL: Bug Tracker, https://github.com/muhammedsural/TSC2018_Design/issues
 Keywords: TSC2018,ETABS,SAP2000,DESIGN,TS500-2000
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,17 @@
 
 # Todo list
 - [x] Design of confining reinforcement in rectangular columns according to TSC2018 .
 - [x] Creation of the steel model with the confined and unconfined mander concrete model specified in ANNEX 5-A of the TSC2018.
 - [x] Creating the spectrum graphs given in section 3  of the TSC2018.
 - [x] Finding the building height class (BYS) and the maximum possible building height according to the information given.
 - [x] Connection with Etabs(CSI product) program and getting results
-- [x] Fibrous polymer calculations added according to TSC2018
+- [x] Calculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Interstory drift check according to TSC2018
 - [ ] Earthquake record selection, acceleration record reading, spectral acceleration, velocity and displacement series extraction and scaling operations.
-- [ ] LCalculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Finding performance targets based on the information provided according to TSC2018
 - [ ] Recommendation of R and D coefficients in accordance with TSC2018.
 - [ ] Finding equivalent lateral loads according to TSC2018.
 - [ ] External forces in cantilever retaining walls according to TBDY2018.
 
 
 # Summary of repo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSC2018_Design Version: 1.1.4 Summary: TSC2018
+Metadata-Version: 2.1 Name: TSC2018_Design Version: 1.1.5 Summary: TSC2018
 design Author-email: Muhammed Sural
 gmail.com> Project-URL: Homepage, https://github.com/muhammedsural/
 TSC2018_Design Project-URL: Bug Tracker, https://github.com/muhammedsural/
 TSC2018_Design/issues Keywords: TSC2018,ETABS,SAP2000,DESIGN,TS500-2000
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -11,27 +11,26 @@
 Requires-Dist: comtypes This repo aims to calculate the topics in TS500-2000
 and TSC2018 by coding them with Python. # Todo list - [x] Design of confining
 reinforcement in rectangular columns according to TSC2018 . - [x] Creation of
 the steel model with the confined and unconfined mander concrete model
 specified in ANNEX 5-A of the TSC2018. - [x] Creating the spectrum graphs given
 in section 3 of the TSC2018. - [x] Finding the building height class (BYS) and
 the maximum possible building height according to the information given. - [x]
-Connection with Etabs(CSI product) program and getting results - [x] Fibrous
-polymer calculations added according to TSC2018 - [ ] Interstory drift check
-according to TSC2018 - [ ] Earthquake record selection, acceleration record
-reading, spectral acceleration, velocity and displacement series extraction and
-scaling operations. - [ ] LCalculation of strength and ductility increase in
-columns confined with fibrous polymer - [ ] Finding performance targets based
-on the information provided according to TSC2018 - [ ] Recommendation of R and
-D coefficients in accordance with TSC2018. - [ ] Finding equivalent lateral
-loads according to TSC2018. - [ ] External forces in cantilever retaining walls
-according to TBDY2018. # Summary of repo ![PyPI - Version](https://
-img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) ![PyPI - Downloads]
-(https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-badge) ![GitHub
-forks](https://img.shields.io/github/forks/muhammedsural/
+Connection with Etabs(CSI product) program and getting results - [x]
+Calculation of strength and ductility increase in columns confined with fibrous
+polymer - [ ] Interstory drift check according to TSC2018 - [ ] Earthquake
+record selection, acceleration record reading, spectral acceleration, velocity
+and displacement series extraction and scaling operations. - [ ] Finding
+performance targets based on the information provided according to TSC2018 -
+[ ] Recommendation of R and D coefficients in accordance with TSC2018. - [ ]
+Finding equivalent lateral loads according to TSC2018. - [ ] External forces in
+cantilever retaining walls according to TBDY2018. # Summary of repo ![PyPI -
+Version](https://img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-
+badge) ![GitHub forks](https://img.shields.io/github/forks/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub contributors](https://
 img.shields.io/github/contributors/muhammedsural/TSC2018_Design?style=for-the-
 badge) ![GitHub stars](https://img.shields.io/github/stars/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub issues](https://img.shields.io/
 github/issues/muhammedsural/TSC2018_Design?style=for-the-badge) ![GitHub
 License](https://img.shields.io/github/license/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub commit activity](https://
```

### Comparing `TSC2018_Design-1.1.4/README.md` & `tsc2018_design-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 # Todo list
 - [x] Design of confining reinforcement in rectangular columns according to TSC2018 .
 - [x] Creation of the steel model with the confined and unconfined mander concrete model specified in ANNEX 5-A of the TSC2018.
 - [x] Creating the spectrum graphs given in section 3  of the TSC2018.
 - [x] Finding the building height class (BYS) and the maximum possible building height according to the information given.
 - [x] Connection with Etabs(CSI product) program and getting results
-- [x] Fibrous polymer calculations added according to TSC2018
+- [x] Calculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Interstory drift check according to TSC2018
 - [ ] Earthquake record selection, acceleration record reading, spectral acceleration, velocity and displacement series extraction and scaling operations.
-- [ ] LCalculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Finding performance targets based on the information provided according to TSC2018
 - [ ] Recommendation of R and D coefficients in accordance with TSC2018.
 - [ ] Finding equivalent lateral loads according to TSC2018.
 - [ ] External forces in cantilever retaining walls according to TBDY2018.
 
 
 # Summary of repo
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
 This repo aims to calculate the topics in TS500-2000 and TSC2018 by coding them
 with Python. # Todo list - [x] Design of confining reinforcement in rectangular
 columns according to TSC2018 . - [x] Creation of the steel model with the
 confined and unconfined mander concrete model specified in ANNEX 5-A of the
 TSC2018. - [x] Creating the spectrum graphs given in section 3 of the TSC2018.
 - [x] Finding the building height class (BYS) and the maximum possible building
 height according to the information given. - [x] Connection with Etabs(CSI
-product) program and getting results - [x] Fibrous polymer calculations added
-according to TSC2018 - [ ] Interstory drift check according to TSC2018 - [ ]
-Earthquake record selection, acceleration record reading, spectral
-acceleration, velocity and displacement series extraction and scaling
-operations. - [ ] LCalculation of strength and ductility increase in columns
-confined with fibrous polymer - [ ] Finding performance targets based on the
-information provided according to TSC2018 - [ ] Recommendation of R and D
-coefficients in accordance with TSC2018. - [ ] Finding equivalent lateral loads
-according to TSC2018. - [ ] External forces in cantilever retaining walls
-according to TBDY2018. # Summary of repo ![PyPI - Version](https://
-img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) ![PyPI - Downloads]
-(https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-badge) ![GitHub
-forks](https://img.shields.io/github/forks/muhammedsural/
+product) program and getting results - [x] Calculation of strength and
+ductility increase in columns confined with fibrous polymer - [ ] Interstory
+drift check according to TSC2018 - [ ] Earthquake record selection,
+acceleration record reading, spectral acceleration, velocity and displacement
+series extraction and scaling operations. - [ ] Finding performance targets
+based on the information provided according to TSC2018 - [ ] Recommendation of
+R and D coefficients in accordance with TSC2018. - [ ] Finding equivalent
+lateral loads according to TSC2018. - [ ] External forces in cantilever
+retaining walls according to TBDY2018. # Summary of repo ![PyPI - Version]
+(https://img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) ![PyPI -
+Downloads](https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-badge) !
+[GitHub forks](https://img.shields.io/github/forks/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub contributors](https://
 img.shields.io/github/contributors/muhammedsural/TSC2018_Design?style=for-the-
 badge) ![GitHub stars](https://img.shields.io/github/stars/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub issues](https://img.shields.io/
 github/issues/muhammedsural/TSC2018_Design?style=for-the-badge) ![GitHub
 License](https://img.shields.io/github/license/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub commit activity](https://
```

### Comparing `TSC2018_Design-1.1.4/pyproject.toml` & `tsc2018_design-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TSC2018_Design"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Muhammed Sural", email="muhammedsural@gmail.com" },
 ]
 description = "TSC2018 design"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/ConfimentBarsRules.py` & `tsc2018_design-1.1.5/src/TSC/Design/ConfimentBarsRules.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,29 +35,36 @@
     s_MiddleConfAreaMax     : float = field(init=False,repr=False)
     s_OtherConfAreaMax      : float = field(init=False,repr=False)
     s_OptEndConfArea        : float = field(init=False,repr=False)
     s_OptMiddleConfArea     : float = field(init=False,repr=False)
 
         
     def Set_Variables(self) -> None:
+        RebarCheck = self.CheckConfinmendRebarDiameter(ConfRebarDia=self.ConfimentRebarDiameter, LongRebarDia=self.LongnitudeRebarDiameter)
+        if RebarCheck != True:
+            return None
         self.Ac                  = self.GetAc(self.Height,self.Width)
         self.Ack                 = self.GetAck(self.Height,self.Width,self.Cover)
         self.bkx                 = self.Get_bk(self.Width,self.Cover)
         self.bky                 = self.Get_bk(self.Height,self.Cover)
         self.ax                  = self.Get_a_i(self.bkx,self.Xkol)
+        GeomCheck                = self.Check_a_i(ai=self.ax , confrebardia=self.ConfimentRebarDiameter)
         self.ay                  = self.Get_a_i(self.bky,self.Ykol)
+        GeomCheck                = self.Check_a_i(ai=self.ay , confrebardia=self.ConfimentRebarDiameter)
+        if GeomCheck != True:
+            return None
         ConfRebarArea            = self.GetRebarArea(self.ConfimentRebarDiameter)
         self.Ashx                = self.GetAshw_i(self.Xkol,ConfRebarArea)
         self.Ashy                = self.GetAshw_i(self.Ykol,ConfRebarArea)
         self.Ash                 = self.Ashx + self.Ashy
         bmin                     = min(self.Height,self.Width)
         bmax                     = max(self.Height,self.Width)
         
         self.EndConfLength       = self.Get_EndRegionConfinmentLength(bmax,self.Ln)
-        self.Lb                  = self.Get_lb(self.Fsy, self.Fctd, self.LongnitudeRebarDiameter)
+        self.Lb                  = self.Get_lb(self.Fsy, self.Fctd, self.LongnitudeRebarDiameter, Nervur=True, LocationClass=1)
         self.MidConfLength       = self.Lb
         self.OtherConfLength     = self.Ln - 2 * self.EndConfLength - self.MidConfLength
 
         self.s_EndConfAreaMax    = self.UcSarilmaBolgesiKontrolleri(self.LongnitudeRebarDiameter,bmin)
         self.s_MiddleConfAreaMax = self.OrtaSarilmaBolgesiKontrolleri(bmin,self.LongnitudeRebarDiameter)
         self.s_OtherConfAreaMax  = self.DigerSarilmaBolgesiKontrolleri(bmin,self.LongnitudeRebarDiameter)
 
@@ -147,20 +154,23 @@
 
     def CheckConfinmendRebarDiameter(self,ConfRebarDia : float, LongRebarDia : float) -> bool:
         if ConfRebarDia < (LongRebarDia/3):
             print(f"Sargı donatısı çapı boyuna donatı çapının üçte birinden az olamaz!!! - TS500-7.4.1")
             return False
         return True
 
-    def Check_a_i(self,ai : float,confrebardia : float):
-        if ai > 25*(confrebardia/10):
+    def Check_a_i(self,ai : float,confrebardia : float) -> bool:
+        if ai > 25*(confrebardia):
             print(f"İlgili doğrultuda kol aralığı izin verilenin sınırın üstünde {ai}mm > {25*confrebardia}mm - TBDY-7.3.4.2")
+            return False
 
         if ai > 300:
             print(f"İlgili doğrultuda kol aralığı izin verilenin sınırın üstünde {ai}mm > 300mm - TS500 7.4.1")
+            return False
+        return True
             
     def CheckNd(self,Nd : float,Ac : float, fck : float) -> bool:
         """Nd değerinin (0.2 * Ac * fck) değerinden büyük veya küçük eşit olma durumunu inceler. Büyükse False küçükse True döndürür.
 
         Args:
             Nd (float): Yük katsayıları ile çarpılmış düşey yükler ve deprem yüklerinin ortak etkisi
                         altında hesaplanan eksenel kuvvet
@@ -188,34 +198,39 @@
         """
         s1 = 50 # TBDY2018
         s2 = 150 # TBDY2018
         s3 = b_min/3 # TBDY2018
         s4 = 6 * LongRebar  # TBDY2018
         s5 = 12 * LongRebar # TS500
         s_max = min(s2,s3,s4,s5)
-
+        print(f"Uç sarılma bölgesi şartları ==> \ns1 = {round(s1,1)}mm, \ns2 = {round(s2,1)}mm, \ns3 = {b_min}/3 = {round(s3,1)}mm, \ns4 = 6 * {LongRebar} = {round(s4,1)}mm, \ns5 = 12 * {LongRebar} = {round(s5,1)}mm \n==> smax = min(s2,s3,s4,s5) = {round(s_max,1)}mm")
+        
         if s_max < s1 :
+            print(f"{s_max} < {s1} olamaz bu nedenle uygulanabilecek etriye aralığı {s1} alınmıştır.")
             s_max = s1
-
+        print("=="*50+"\n")
         return s_max
 
     def OrtaSarilmaBolgesiKontrolleri(self,b_min : float,LongRebar : int) -> float:
         s1 = 150
         s2 = b_min/3
         s3 = 12 * LongRebar # TS500
         # s4 = 6 * LongRebar # TBDY2018
         s_max = min(s1,s2,s3)
-
+        print(f"Orta sarılma bölgesi şartları ==> \ns1 = {round(s1,1)}mm, \ns2 = {b_min} / 3 = {round(s2,1)}mm, \ns3 = 12 * {LongRebar}  = {round(s3,1)}mm \n==> smax = min(s1,s2,s3) = {round(s_max,1)}mm")
+        print("=="*50+"\n")
         return s_max
 
     def DigerSarilmaBolgesiKontrolleri(self, b_min : float,LongRebar : int) -> float:
         s1 = 200
         s2 = b_min/2
         s3 = math.floor(12 * LongRebar) # TS500
         s_max = min(s1,s2,s3)
+        print(f"Sarılma bölgesi dışı şartları ==> \ns1 = {round(s1,1)}mm, \ns2 = {b_min} / 2 = {round(s2,1)}mm, \ns3 = 12 * {LongRebar}  = {round(s3,1)}mm \n==> smax = min(s1,s2,s3) = {round(s_max,1)}mm")
+        print("=="*50+"\n")
         return s_max
     
     def MinEnineDonatiOraniDikdörtgen(self,s : float, b_kx : float,b_ky : float, Ac : float, Ack : float, fck : float, fywk : float,NdControl : bool) -> float:
         """_summary_
         Args:
             s   (float) : Etriye aralığı 
             b_kx(float) : X doğrultusu için, kolon veya perde uç bölgesi
@@ -241,27 +256,42 @@
 
         Ash = max(Ash1,Ash2)
         if NdControl:
             Ash = Ash * 2/3        
         return Ash
 
     def OptimizeConfinmentRebarSpace(self,smax : float,Ash : float, Nd : float, Ac : float, fck : float, fywk : float, Ack : float, bkx : float, bky : float) -> int:
+        """Kesitte atılabilecek optimize etriye aralığını herhangi bir bölge olabilir
+
+        Args:
+            smax (float): Maximum atılabilecek etriye aralığı
+            Ash (float): Enine donatı oranı
+            Nd (float): Eksenel kuvvet N
+            Ac (float): Kesit alanı
+            fck (float): Karakteristik basınç dayanımı
+            fywk (float): Enine donatı akma gerilmesi MPa
+            Ack (float): Çekirdek beton alanı mm2
+            bkx (float): çekirdek beton genişliği
+            bky (float): Çekirdek beton yüksekliği
+
+        Returns:
+            int: Etriye aralığı
+        """
         s    = [i for i in range(50,210)]   # cm
         s_ideal = 0
         for s_opt in s :
             if s_opt > smax:
                 break
             NdControl = self.CheckNd(Nd,Ac,fck)
             Ashmin_dikd = self.MinEnineDonatiOraniDikdörtgen(s_opt,bkx,bky,Ac,Ack,fck,fywk,NdControl)
             if Ash < Ashmin_dikd:
                 if s_opt == 50:
                     #info :  İlk iterasyonda Ash_min değerinin altında kalıyorsa diğerlerinde zaten sağlayamaz s_opt değeri 50mm e eşitlenip uyarı verilir.
                     print(f"Ash = {Ash}mm2 < Ash_min = {Ashmin_dikd}mm2 kesitteki çiroz,etriye arttırılmalı ve/veya sargı donatı çapı büyütülmeli...")
-                    break
-                s_ideal = s_opt
+                    s_ideal = 50
                 break
             s_ideal = s_opt
 
         return s_ideal
 
     def Get_lb(self, fsy : float, fctd : float, LognRebarDia : float, Nervur : bool = True, LocationClass : int = 2):
         """TS 500’de çekme donatısı için verilen kenetlenme boyunu hesaplar
@@ -275,31 +305,39 @@
 
         Raises:
             ValueError: Konum bilgisi yanlışsa döndürülür.
 
         Returns:
             _type_: kenetlenme boyu
         """
-        # 
         
         lb = 0.12 * (fsy/fctd) * LognRebarDia
-        minlimit = 20 * LognRebarDia
+        print(f"Lb = 0.12 * (fsy/fctd) * LognRebarDia = 0.12 * {(fsy/fctd)} * {LognRebarDia} = {lb}mm")
+        
+        minlimit = 20 * LognRebarDia # Bu sınır TS500 de 20 * fi_boyunadonatı dır.
         
         if lb < minlimit :
+            print(f"Lb = {lb} < {minlimit} = 20*LognRebarDia ==> Lb = {minlimit} \n")
             lb = minlimit
         
         if LocationClass == 1 :
+            print(f"LocationClass = 1 < ==> Lb = 1.4 * Lb = {1.4*lb} \n")
             lb = 1.4 * lb
             
         if LocationClass != 1 and LocationClass != 2:
-            raise ValueError("Konum tanımı 1 veya 2 olmalıdır...")
+            raise ValueError("Konum tanımı 1 veya 2 olmalıdır...\n")
         
         if Nervur != True:
+            print(f"Boyuna donatı nervürsüz ==> Lb = 2 * Lb = {2*lb} ")
             lb = 2 * lb
-        
+
+        if lb < 40 * LognRebarDia:
+            lb = 40 * LognRebarDia # ACI19 - R25.4.2.3 de ilgili configirasyonda 47 db minimum boy çıkmaktadır. TS için 40 db gelmektedir.
+
+        print("=="*50+"\n")
         return lb
     
     def Get_EndRegionConfinmentLength(self, b_max : float, ln : float):
         """Uç sarılma bölgelerinin uzunluklarını hesaplar.
 
         Args:
             b_max (float): kolon en büyük kesit boyutu
@@ -308,14 +346,16 @@
         Returns:
             _type_: Uç sarılma bölgelerinin uzunlukları
         """
         l1 = 1.5 * b_max
         l2 = 500
         l3 = ln/6
         l = max(l1,l2,l3)
+        print(f"Uç sarılma bölgesi uzunluk şartları ==> \nL1 = 1.5 * b_max = 15 * {b_max} = {round(l1,1)}mm, \nL2 = {round(l2,1)}mm, \nL3 = Ln/6 = {ln}/6 = {round(l3,1)}mm \n==> Lmax = max(L1,L2,L3) = {round(l,1)}mm")
+        print("=="*50+"\n")
         return l
     
     def Get_DesignConfinment(self,
                              TieRebarDiameter : int,
                              bmax : float, 
                              ln : float, 
                              UcSarilmaBolgesiUzunlugu : float, 
@@ -344,9 +384,26 @@
         OrtaSarilmaBolgesiEtriyeAdeti = math.ceil(OrtaSarilmaBolgesiUzunlugu / s_OptMiddleConfArea) + 1
         SarilmaBolgesiDisindaEtriyeAdeti = math.ceil(SarilmaBolgesiDisindaKalanUzunluk / s_OtherConfAreaMax) + 2
         
         # BUG iç etriye veya çirozlar sayılmamış
         EtriyeAdeti = 2*UcSarilmaBolgesiEtriyeAdeti + OrtaSarilmaBolgesiEtriyeAdeti + SarilmaBolgesiDisindaEtriyeAdeti
         print(f"Kolon Serbest Bölgesindeki Etriye Adeti - Etriye Çapi / SarılmaDışıAralık / OrtaSarılmadakiAralık / UçSarılmaAralık = {EtriyeAdeti} - ∅{TieRebarDiameter} / {math.floor(s_OtherConfAreaMax/10)} / {math.floor(s_OptMiddleConfArea/10)} / {math.floor(s_OptEndConfArea/10)}")
         
-        
 
+
+# if __name__ == "__main__":
+#     Cbar = ConfimentDesign(
+#                             Nd                      = 22703.2*10**4,
+#                             Fsy                     = 420 ,
+#                             Fctd                    = 2.1,
+#                             Ln                      = 2200,            
+#                             Width                   = 450,
+#                             Height                  = 400,
+#                             Cover                   = 23,
+#                             Xkol                    = 4,
+#                             Ykol                    = 3,
+#                             Fck                     = 35,
+#                             Fywk                    = 420,
+#                             ConfimentRebarDiameter  = 10,
+#                             LongnitudeRebarDiameter = 14)
+#     Cbar.Set_Variables()
+#     print(f"Uç sarılma bölgesi uzunluğu = {Cbar.EndConfLength}, Orta sarılma bölgesi uzunluğu = {Cbar.MidConfLength}, Kalan uzunluk = {Cbar.OtherConfLength}")
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/Definitions.py` & `tsc2018_design-1.1.5/src/TSC/Design/Definitions.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/Frp.py` & `tsc2018_design-1.1.5/src/TSC/Design/Frp.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/GlobalParamCheck.py` & `tsc2018_design-1.1.5/src/TSC/Design/GlobalParamCheck.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/MaterialModels.py` & `tsc2018_design-1.1.5/src/TSC/Design/MaterialModels.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/ResponseSpectra.py` & `tsc2018_design-1.1.5/src/TSC/Design/ResponseSpectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,15 +756,23 @@
         targetSa = 0
         for index,T_series in enumerate(Periods):
             if round(T_series,2) == T:
                 targetSa = Accelertions[index]
                 break
         return round(targetSa,4)
 
-
+    def ChangeTimeSeriesForPGA(TimeSeries : pd.DataFrame,targetPGA : float) -> pd.DataFrame:
+        """ Zaman serisini PGA değerine göre verilen ivme değeri ile orantılayarak yeniden oluşturur."""
+        realPGA = TimeSeries.Acceleration.max()
+        coef = targetPGA/realPGA
+        newTimeSeries = [acc*coef for acc in TimeSeries.Acceleration]
+        TimeSeries["ChangedAcc"] = newTimeSeries
+        del newTimeSeries
+        return TimeSeries
+    
 # def main() ->None:
 #     # SeismicVariables = SeismicInputs(lat = 38.12949,lon = 32.45234,soil = "ZC",intensity = "DD2")
 #     # print(SeismicVariables)
 #     # print("="*80)
     
 
 #     # RCBuilding = SeismicResistanceBuildingInputs(Hn=70,
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/Design/SeismicLoad.py` & `tsc2018_design-1.1.5/src/TSC/Design/SeismicLoad.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/AnalysisResult.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/AnalysisResult.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from TSC.MSCSI.ErrorHandler import CustomCommentError
 
 # Tamamlananlar
 @dataclass
 class BaseReact:
      """Class for base_react return"""
      number_results      : int     = field(default_factory=int)
-     load_case           : [str]   = field(default_factory=list)
-     step_type           : [str]   = field(default_factory=list)
-     step_number         : [float] = field(default_factory=list)
-     force_x             : [float] = field(default_factory=list)
-     force_y             : [float] = field(default_factory=list)
-     force_z             : [float] = field(default_factory=list)
-     moment_x            : [float] = field(default_factory=list)
-     moment_y            : [float] = field(default_factory=list)
-     moment_z            : [float] = field(default_factory=list)
+     load_case           : list[str]   = field(default_factory=list)
+     step_type           : list[str]   = field(default_factory=list)
+     step_number         : list[float] = field(default_factory=list)
+     force_x             : list[float] = field(default_factory=list)
+     force_y             : list[float] = field(default_factory=list)
+     force_z             : list[float] = field(default_factory=list)
+     moment_x            : list[float] = field(default_factory=list)
+     moment_y            : list[float] = field(default_factory=list)
+     moment_z            : list[float] = field(default_factory=list)
      x_coordinate        : float   = field(default_factory=float)
      y_coordinate        : float   = field(default_factory=float)
      z_coordinate        : float   = field(default_factory=float)
      
      def __repr__(self) -> str:
           return f"Load cases : {self.load_case}\nForce_x : {self.force_x}\nForce_y : {self.force_y}\nForce_z : {self.force_z}\nMoment_x : {self.moment_x}\nMoment_y : {self.moment_y}\nMoment_z : {self.moment_z}"
 
@@ -357,24 +357,24 @@
                This is an array of the displacements in the Y direction [L] 
           Delta_Z
                This is an array of the displacements in the Z direction [L] 
 
      """
        
      NumberResults       : int     = field(default_factory=int)
-     Story               : [str]   = field(default_factory=list)
-     LoadCase            : [str]   = field(default_factory=list)
-     StepType            : [str]   = field(default_factory=list)
-     StepNum             : [float] = field(default_factory=list)
-     Direction           : [str]   = field(default_factory=list)
-     Drift               : [float] = field(default_factory=list)
-     Label               : [str]   = field(default_factory=list)
-     Delta_X             : [float] = field(default_factory=list)
-     Delta_Y             : [float] = field(default_factory=list)
-     Delta_Z             : [float] = field(default_factory=list)
+     Story               : list[str]   = field(default_factory=list)
+     LoadCase            : list[str]   = field(default_factory=list)
+     StepType            : list[str]   = field(default_factory=list)
+     StepNum             : list[float] = field(default_factory=list)
+     Direction           : list[str]   = field(default_factory=list)
+     Drift               : list[float] = field(default_factory=list)
+     Label               : list[str]   = field(default_factory=list)
+     Delta_X             : list[float] = field(default_factory=list)
+     Delta_Y             : list[float] = field(default_factory=list)
+     Delta_Z             : list[float] = field(default_factory=list)
      
      def __repr__(self) -> str:
           return f"Story : {self.Story}\nLoad cases : {self.LoadCase}\nDirection : {self.Direction}\Drift : {self.Drift}\nNodes : {self.Label}\nDelta_X : {self.Delta_X}\nDelta_Y : {self.Delta_Y}\nDelta_Z : {self.Delta_Z}"
 
      def to_dict(self) -> dict:
           return asdict(self)
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Analyze.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Analyze.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/CaseStaticNonlinear.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/CaseStaticNonlinear.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Combo.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Combo.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Connector.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,8 +71,11 @@
         ret = SapModel.InitializeNewModel()
         if ret != 0:
             raise ApiReturnError(ret)
         
         ret = SapModel.File.OpenFile(ModelPath)
         if ret != 0:
             raise ApiReturnError(ret)
-    return SapModel,myETABSObject
+    return SapModel,myETABSObject
+
+# if __name__ == "__main__":
+#     MySapModel,myETABSObject  = ConnectionEtabs()
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Database.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Database.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Enums.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Enums.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/ErrorHandler.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/ErrorHandler.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/File.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/File.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Frame.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Frame.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/LoadPattern.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,134 @@
 
 from dataclasses import dataclass
-
-from TSC.MSCSI.Enums import eLoadPatternType
+from TSC.MSCSI.Enums import eReturnCode, eUnits
 from TSC.MSCSI.ErrorHandler import ApiReturnError
 
 
 @dataclass
-class LoadPattern:
-    RefApi : object # SapModel.LoadPatterns
-    # AutoSeismic : cAutoSeismic 
-    # AutoWind    : cAutoWind
-
-    def Add(self,Name : str, MyType : eLoadPatternType, SelfWTMultiplier : float = 0, AddAnalysisCase : bool = True) -> None|ApiReturnError:
-        """Adds a new load pattern.
+class SapModel:
+    RefApi      : object
 
+    def GetDatabaseUnits(self) -> None:
+         val = self.RefApi.GetDatabaseUnits()
+         for unitName,unitValue in zip(eUnits._member_map_.keys(),eUnits._member_map_.values()):
+            if val == unitValue.value: 
+                 print(unitName)
+                 break
+            
+    def GetDatabaseUnits_2(self,forceUnits : int, lengthUnits : int, temperatureUnits : int) -> list:
+         val = self.RefApi.GetDatabaseUnits_2(forceUnits,lengthUnits,temperatureUnits)
+         return val
+    
+    def GetMergeTol(self, MergeTol : float) -> list:
+         val = self.RefApi.GetMergeTol(MergeTol)
+         return val
+
+    def GetModelFilename(self,IncludePath  : bool) -> str:
+        """Returns a string that represents the filename of the current model, with or without the full path. 
+            Method testi yapılmadı sıkıntı çıkabilir...
         Args:
-            Name (str): The name for the new load pattern.
-            MyType (eLoadPatternType): This is one of the items in the eLoadPatternType enumeration. 
-            SelfWTMultiplier (float, optional): The self weight multiplier for the new load pattern. . Defaults to 0.
-            AddAnalysisCase (bool, optional): If this item is True, a linear static load case corresponding to the new load pattern is added.Defaults to True.
+            IncludePath (bool): A boolean (True or False) value. When this item is True, the returned filename includes the full path where the file is located. 
 
-        Raises:
-            ApiReturnError: Error descriptions
+        """
+        Filename = self.RefApi.GetModelFilename(IncludePath)
+        return Filename
+    
+    def GetModelFilename(self) -> str:
+        """Returns a string that represents the filepath of the current model 
 
         Returns:
-            None|ApiReturnError
+            str: Returns a string that represents the filepath of the current model 
         """
-        result = self.RefApi.Add(Name,MyType,SelfWTMultiplier,AddAnalysisCase)
-        if result != 0:
-            raise ApiReturnError(result)
-        else:
-            print("Operation completed...")
-
-    def ChangeName(self, Name : str, NewName : str) -> None|ApiReturnError:
-        """Applies a new name to a load pattern.
+        Filepath = self.RefApi.GetModelFilepath()
+        return Filepath
+    
+    def GetModelIsLocked(self) -> bool:
+        return self.RefApi.GetModelIsLocked()
+    
+    def GetPresentCoordSystem(self) -> str:
+        return self.RefApi.GetPresentCoordSystem()
+    
+    def GetPresentUnits(self) -> None:
+        val = self.RefApi.GetPresentUnits()        
+        for unitName,unitValue in zip(eUnits._member_map_.keys(),eUnits._member_map_.values()):
+            if val == unitValue.value: 
+                 print(unitName)
+                 break
+    
+    def GetPresentUnits_2(self, forceUnits:int, lengthUnits:int, temperatureUnits:int) -> list:
+         val = self.RefApi.GetPresentUnits_2(forceUnits,lengthUnits,temperatureUnits)
+         return val
+    
+    def GetProgramInfo(self, ProgramName: str, ProgramVersion : str, ProgramLevel : str) -> int:
+         val = self.RefApi.GetProgramInfo(ProgramName,ProgramVersion,ProgramLevel)
+         return val
+    
+    def GetProjectInfo(self, NumberItems : int, Item : str, Data : str) -> int:
+         val = self.RefApi.GetProjectInfo(NumberItems,Item,Data)
+         return val
+    
+    def GetVersion(self, Version: str, MyVersionNumber : float) -> int:
+         val = self.RefApi.GetVersion(Version,MyVersionNumber)
+         return val
+    
+    def InitializeNewModel(self, Units : int = eUnits.kN_m_C.value):
+         val = self.RefApi.InitializeNewModel(Units)
+         if val != 0:
+            raise ApiReturnError(val)
+         
+    def SetMergeTol(self, MergeTol: float) -> None | ApiReturnError:
+         val = self.RefApi.SetMergeTol(MergeTol)
+         if val != 0:
+            raise ApiReturnError(val)
+    
+    def SetModelIsLocked(self, Lockit : bool) -> None | ApiReturnError:
+         val = self.RefApi.SetModelIsLocked(Lockit)
+         if val != 0:
+            raise ApiReturnError(val)
+    
+    def SetPresentUnits(self,Units : int) -> None | ApiReturnError:
+         val = self.RefApi.SetPresentUnits(Units)
+         if val != 0:
+            raise ApiReturnError(val)
+    
+    def SetPresentUnits_2(self, forceUnits:int, lengthUnits:int, temperatureUnits:int) -> None | ApiReturnError:
+         val = self.RefApi.SetPresentUnits_2(forceUnits,lengthUnits,temperatureUnits)
+         if val != 0:
+            raise ApiReturnError(val)
+    
+    def SetProjectInfo(self,Item : str, Data : str) -> None | ApiReturnError:
+        """_summary_
 
         Args:
-            Name (str): The name of a defined load pattern.
-            NewName (str): The new name for the load pattern.
+            Item (str): _description_
+            Data (str): _description_
 
         Raises:
-            ApiReturnError: Error descriptions
+            CustomCommentError: _description_
+            CustomCommentError: _description_
 
         Returns:
-            None|ApiReturnError
+            int: _description_
         """
-        result = self.RefApi.ChangeName(Name,NewName)
-        if result != 0:
-            raise ApiReturnError(result)
-        else:
-            print("Operation completed...")
-
-    def Count(self) -> int:
-        """Retrieves the number of defined load patterns."""
-        result = self.RefApi.Count()
-        return result
 
-    def Delete(self,Name : str) -> None|ApiReturnError:
-        """Deletes the specified load pattern.  
-
-        Args:
-            Name (str): The name of a defined load pattern.
-        """
-        result = self.RefApi.Delete(Name)
-        if result != 0:
-            raise ApiReturnError(result)
-        else:
-            print("Operation completed...")
-
-    def GetAutoSeismicCode(self,Name : str):
-        """Retrieves the code name used for auto seismic parameters in Quake-type load patterns."""  
-        CodeName = str()
-        result = self.RefApi.GetAutoSeismicCode(Name,CodeName)
-        return result
-
-    def GetAutoWindCode(self,Name : str):
-        """Retrieves the code name used for auto wind parameters in Wind-type load patterns.  """
-        CodeName = str()
-        result = self.RefApi.GetAutoSeismicCode(Name,CodeName)
-        return result
-    
-    def GetLoadType(self,Name : str) -> None|ApiReturnError:
-        """Retrieves the load type for a specified load pattern.  """
-        MyType = int()
-        result = self.RefApi.GetLoadType(Name,MyType)
-        return result
-
-    def GetNameList(self) -> None|ApiReturnError:
-        """Retrieves the names of all defined load cases.  """
-        NumberNames = int()
-        MyName = list([])
-        retVal = 0
-        result = [NumberNames,MyName,retVal]
-        result = self.RefApi.GetNameList(NumberNames,MyName)
-        if result[-1] != 0:
-            raise ApiReturnError(result[-1])
-        else:
-            print("Operation completed...")
-            return result
-
-    def GetSelfWTMultiplier(self,Name : str) -> None|ApiReturnError:
-        """Retrieves the self weight multiplier for a specified load pattern."""
-        SelfWTMultiplier = float()
-        retVal = 0
-        result = [SelfWTMultiplier,retVal]
-        result = self.RefApi.GetSelfWTMultiplier(Name,SelfWTMultiplier)
-        if result[-1] != 0:
-            raise ApiReturnError(result[-1])
-        else:
-            print("Operation completed...")
-            return result
-
-    def SetLoadType(self,Name : str,MyType : eLoadPatternType) -> None|ApiReturnError:
-        """Assigns a load type to a load pattern."""
-        result = self.RefApi.SetLoadType(Name,MyType)
-        if result != 0:
-            raise ApiReturnError(result)
-        else:
-            print("Operation completed...")
-        
-    def SetSelfWTMultiplier(self, Name : str, SelfWTMultiplier : float) -> None|ApiReturnError:
-        """Assigns a self weight multiplier to a load case."""
-        result = self.RefApi.SetLoadType(Name,SelfWTMultiplier)
-        if result != 0:
-            raise ApiReturnError(result)
-        else:
-            print("Operation completed...")
+        val = self.RefApi.SetProjectInfo(Item,Data)
+        if val != 0:
+            raise ApiReturnError(val)
+    
+    def TreeIsUpdateSuspended(self,IsSuspended : bool):
+         val = self.RefApi.TreeIsUpdateSuspended(IsSuspended)
+         if val != 0:
+            raise ApiReturnError(val)
+         pass
+    
+    def TreeResumeUpdateData(self):
+         val = self.RefApi.TreeResumeUpdateData()
+         if val != 0:
+            raise ApiReturnError(val)
+         pass
+    
+    def TreeSuspendUpdateData(self,updateAtResume):
+         val = self.RefApi.TreeSuspendUpdateData(updateAtResume)
+         if val != 0:
+            raise ApiReturnError(val)
+         pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/MaterialProp.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/MaterialProp.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/MSCSI/Story.py` & `tsc2018_design-1.1.5/src/TSC/MSCSI/Story.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC/Utility/Decorators.py` & `tsc2018_design-1.1.5/src/TSC/Utility/Decorators.py`

 * *Files identical despite different names*

### Comparing `TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/PKG-INFO` & `tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSC2018_Design
-Version: 1.1.4
+Version: 1.1.5
 Summary: TSC2018 design
 Author-email: Muhammed Sural <muhammedsural@gmail.com>
 Project-URL: Homepage, https://github.com/muhammedsural/TSC2018_Design
 Project-URL: Bug Tracker, https://github.com/muhammedsural/TSC2018_Design/issues
 Keywords: TSC2018,ETABS,SAP2000,DESIGN,TS500-2000
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,18 +24,17 @@
 
 # Todo list
 - [x] Design of confining reinforcement in rectangular columns according to TSC2018 .
 - [x] Creation of the steel model with the confined and unconfined mander concrete model specified in ANNEX 5-A of the TSC2018.
 - [x] Creating the spectrum graphs given in section 3  of the TSC2018.
 - [x] Finding the building height class (BYS) and the maximum possible building height according to the information given.
 - [x] Connection with Etabs(CSI product) program and getting results
-- [x] Fibrous polymer calculations added according to TSC2018
+- [x] Calculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Interstory drift check according to TSC2018
 - [ ] Earthquake record selection, acceleration record reading, spectral acceleration, velocity and displacement series extraction and scaling operations.
-- [ ] LCalculation of strength and ductility increase in columns confined with fibrous polymer
 - [ ] Finding performance targets based on the information provided according to TSC2018
 - [ ] Recommendation of R and D coefficients in accordance with TSC2018.
 - [ ] Finding equivalent lateral loads according to TSC2018.
 - [ ] External forces in cantilever retaining walls according to TBDY2018.
 
 
 # Summary of repo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSC2018_Design Version: 1.1.4 Summary: TSC2018
+Metadata-Version: 2.1 Name: TSC2018_Design Version: 1.1.5 Summary: TSC2018
 design Author-email: Muhammed Sural
 gmail.com> Project-URL: Homepage, https://github.com/muhammedsural/
 TSC2018_Design Project-URL: Bug Tracker, https://github.com/muhammedsural/
 TSC2018_Design/issues Keywords: TSC2018,ETABS,SAP2000,DESIGN,TS500-2000
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -11,27 +11,26 @@
 Requires-Dist: comtypes This repo aims to calculate the topics in TS500-2000
 and TSC2018 by coding them with Python. # Todo list - [x] Design of confining
 reinforcement in rectangular columns according to TSC2018 . - [x] Creation of
 the steel model with the confined and unconfined mander concrete model
 specified in ANNEX 5-A of the TSC2018. - [x] Creating the spectrum graphs given
 in section 3 of the TSC2018. - [x] Finding the building height class (BYS) and
 the maximum possible building height according to the information given. - [x]
-Connection with Etabs(CSI product) program and getting results - [x] Fibrous
-polymer calculations added according to TSC2018 - [ ] Interstory drift check
-according to TSC2018 - [ ] Earthquake record selection, acceleration record
-reading, spectral acceleration, velocity and displacement series extraction and
-scaling operations. - [ ] LCalculation of strength and ductility increase in
-columns confined with fibrous polymer - [ ] Finding performance targets based
-on the information provided according to TSC2018 - [ ] Recommendation of R and
-D coefficients in accordance with TSC2018. - [ ] Finding equivalent lateral
-loads according to TSC2018. - [ ] External forces in cantilever retaining walls
-according to TBDY2018. # Summary of repo ![PyPI - Version](https://
-img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) ![PyPI - Downloads]
-(https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-badge) ![GitHub
-forks](https://img.shields.io/github/forks/muhammedsural/
+Connection with Etabs(CSI product) program and getting results - [x]
+Calculation of strength and ductility increase in columns confined with fibrous
+polymer - [ ] Interstory drift check according to TSC2018 - [ ] Earthquake
+record selection, acceleration record reading, spectral acceleration, velocity
+and displacement series extraction and scaling operations. - [ ] Finding
+performance targets based on the information provided according to TSC2018 -
+[ ] Recommendation of R and D coefficients in accordance with TSC2018. - [ ]
+Finding equivalent lateral loads according to TSC2018. - [ ] External forces in
+cantilever retaining walls according to TBDY2018. # Summary of repo ![PyPI -
+Version](https://img.shields.io/pypi/v/TSC2018_Design?style=for-the-badge) !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/TSC2018_Design?style=for-the-
+badge) ![GitHub forks](https://img.shields.io/github/forks/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub contributors](https://
 img.shields.io/github/contributors/muhammedsural/TSC2018_Design?style=for-the-
 badge) ![GitHub stars](https://img.shields.io/github/stars/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub issues](https://img.shields.io/
 github/issues/muhammedsural/TSC2018_Design?style=for-the-badge) ![GitHub
 License](https://img.shields.io/github/license/muhammedsural/
 TSC2018_Design?style=for-the-badge) ![GitHub commit activity](https://
```

### Comparing `TSC2018_Design-1.1.4/src/TSC2018_Design.egg-info/SOURCES.txt` & `tsc2018_design-1.1.5/src/TSC2018_Design.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,9 @@
 src/TSC/Utility/__init__.py
 src/TSC2018_Design.egg-info/PKG-INFO
 src/TSC2018_Design.egg-info/SOURCES.txt
 src/TSC2018_Design.egg-info/dependency_links.txt
 src/TSC2018_Design.egg-info/requires.txt
 src/TSC2018_Design.egg-info/top_level.txt
 tests/test_FRP.py
+tests/test_MSCSI_LoadCase.py
 tests/test_TSCConfinmentBarsRules.py
```

### Comparing `TSC2018_Design-1.1.4/tests/test_TSCConfinmentBarsRules.py` & `tsc2018_design-1.1.5/tests/test_TSCConfinmentBarsRules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import math
-from src.Design.ConfimentBarsRules import ConfimentDesign
+from TSC.Design.ConfimentBarsRules import ConfimentDesign
 
 """Units N,mm"""
 Nd                      = 16000 
 B                       = 400
 H                       = 400
 s                       = 80
 TieRebarDiameter        = 8
```

