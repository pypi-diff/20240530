# Comparing `tmp/attpc_engine-0.1.0.tar.gz` & `tmp/attpc_engine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attpc_engine-0.1.0.tar", last modified: Tue May 28 18:51:45 2024, max compression
+gzip compressed data, was "attpc_engine-0.1.2.tar", last modified: Thu May 30 15:31:21 2024, max compression
```

## Comparing `attpc_engine-0.1.0.tar` & `attpc_engine-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/LICENSE
--rw-r--r--   0        0        0       52 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/README.md
--rw-r--r--   0        0        0      849 2024-05-28 18:51:45.403875 attpc_engine-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       92 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/src/attpc_engine/__init__.py
--rw-r--r--   0        0        0      309 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/src/attpc_engine/detector/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/src/attpc_engine/detector/beam_pads.py
--rw-r--r--   0        0        0      847 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/src/attpc_engine/detector/constants.py
--rw-r--r--   0        0        0        0 2024-05-28 18:51:31.876005 attpc_engine-0.1.0/src/attpc_engine/detector/data/__init__.py
--rw-r--r--   0        0        0  1847335 2024-05-28 18:51:31.888005 attpc_engine-0.1.0/src/attpc_engine/detector/data/pad_grid.npz
--rw-r--r--   0        0        0   213104 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/data/padxy.csv
--rw-r--r--   0        0        0     6908 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/parameters.py
--rw-r--r--   0        0        0     1656 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/response.py
--rw-r--r--   0        0        0    12589 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/simulator.py
--rw-r--r--   0        0        0     6935 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/solver.py
--rw-r--r--   0        0        0    11436 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/transporter.py
--rw-r--r--   0        0        0     2757 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/detector/writer.py
--rw-r--r--   0        0        0      298 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/kinematics/__init__.py
--rw-r--r--   0        0        0     2450 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/kinematics/convert_kinematics.py
--rw-r--r--   0        0        0     2341 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/kinematics/excitation.py
--rw-r--r--   0        0        0    17339 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/kinematics/pipeline.py
--rw-r--r--   0        0        0     9911 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/src/attpc_engine/kinematics/reaction.py
--rw-r--r--   0        0        0        0 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1338 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/tests/test_detector.py
--rw-r--r--   0        0        0     5198 2024-05-28 18:51:31.892005 attpc_engine-0.1.0/tests/test_kinematics.py
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 attpc_engine-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-30 15:31:09.598547 attpc_engine-0.1.2/LICENSE
+-rw-r--r--   0        0        0       52 2024-05-30 15:31:09.598547 attpc_engine-0.1.2/README.md
+-rw-r--r--   0        0        0      849 2024-05-30 15:31:21.674754 attpc_engine-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-05-30 15:31:09.602547 attpc_engine-0.1.2/src/attpc_engine/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-30 15:31:09.602547 attpc_engine-0.1.2/src/attpc_engine/detector/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-30 15:31:09.602547 attpc_engine-0.1.2/src/attpc_engine/detector/beam_pads.py
+-rw-r--r--   0        0        0      847 2024-05-30 15:31:09.602547 attpc_engine-0.1.2/src/attpc_engine/detector/constants.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:31:09.602547 attpc_engine-0.1.2/src/attpc_engine/detector/data/__init__.py
+-rw-r--r--   0        0        0  1847335 2024-05-30 15:31:09.614548 attpc_engine-0.1.2/src/attpc_engine/detector/data/pad_grid.npz
+-rw-r--r--   0        0        0   213104 2024-05-30 15:31:09.614548 attpc_engine-0.1.2/src/attpc_engine/detector/data/padxy.csv
+-rw-r--r--   0        0        0     6908 2024-05-30 15:31:09.614548 attpc_engine-0.1.2/src/attpc_engine/detector/parameters.py
+-rw-r--r--   0        0        0     1656 2024-05-30 15:31:09.614548 attpc_engine-0.1.2/src/attpc_engine/detector/response.py
+-rw-r--r--   0        0        0    12589 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/detector/simulator.py
+-rw-r--r--   0        0        0     6935 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/detector/solver.py
+-rw-r--r--   0        0        0    11436 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/detector/transporter.py
+-rw-r--r--   0        0        0     2757 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/detector/writer.py
+-rw-r--r--   0        0        0      298 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/kinematics/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/kinematics/convert_kinematics.py
+-rw-r--r--   0        0        0     2341 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/kinematics/excitation.py
+-rw-r--r--   0        0        0    17335 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/kinematics/pipeline.py
+-rw-r--r--   0        0        0     9911 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/src/attpc_engine/kinematics/reaction.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1338 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/tests/test_detector.py
+-rw-r--r--   0        0        0     5198 2024-05-30 15:31:09.618548 attpc_engine-0.1.2/tests/test_kinematics.py
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 attpc_engine-0.1.2/PKG-INFO
```

### Comparing `attpc_engine-0.1.0/LICENSE` & `attpc_engine-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/pyproject.toml` & `attpc_engine-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "attpc_engine"
-version = "0.1.0"
+version = "0.1.2"
 description = "AT-TPC Monte-Carlo simulation engine"
 authors = [
     { name = "Gordon McCann", email = "gordonmccann215@gmail.com" },
     { name = "Zach Serikow", email = "zachserikow@gmail.com" },
 ]
 dependencies = [
     "spyral-utils>=1.0.0",
```

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/beam_pads.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/beam_pads.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/constants.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/constants.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/data/pad_grid.npz` & `attpc_engine-0.1.2/src/attpc_engine/detector/data/pad_grid.npz`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/data/padxy.csv` & `attpc_engine-0.1.2/src/attpc_engine/detector/data/padxy.csv`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/parameters.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/parameters.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/response.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/response.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/simulator.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/simulator.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/solver.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/solver.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/transporter.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/transporter.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/detector/writer.py` & `attpc_engine-0.1.2/src/attpc_engine/detector/writer.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/kinematics/convert_kinematics.py` & `attpc_engine-0.1.2/src/attpc_engine/kinematics/convert_kinematics.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/kinematics/excitation.py` & `attpc_engine-0.1.2/src/attpc_engine/kinematics/excitation.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/src/attpc_engine/kinematics/pipeline.py` & `attpc_engine-0.1.2/src/attpc_engine/kinematics/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 ):
                     raise PipelineError(
                         "Broken step in pipeline! Step 0 residual does not match to Step 1 parent!"
                     )
             else:
                 if (
                     prev_step.residual_2.isotopic_symbol
-                    != cur_step.residual_2.isotopic_symbol
+                    != cur_step.parent.isotopic_symbol
                 ):
                     raise PipelineError(
                         f"Broken step in pipeline! Step {idx-1} residual_2 does not match Step {idx} parent!"
                     )
             self.decays.append(cur_step)
 
         returned_nuclei = 4 + (len(steps) - 1) * 2
```

### Comparing `attpc_engine-0.1.0/src/attpc_engine/kinematics/reaction.py` & `attpc_engine-0.1.2/src/attpc_engine/kinematics/reaction.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/tests/test_detector.py` & `attpc_engine-0.1.2/tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `attpc_engine-0.1.0/tests/test_kinematics.py` & `attpc_engine-0.1.2/tests/test_kinematics.py`

 * *Files identical despite different names*

